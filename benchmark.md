# Benchmark

## Methode

- input => a JSON file of 100.000 user-agents
- filter => useragent + ruby to add timestamp marker
- output => a JSON file
- Use Drill to query time_start - time_end

```
input
{
    file
    {
        path => "/opt/logstash-filter-useragent/dev/input.json"
        start_position => "beginning"
        codec => json
        ignore_older => -1
        sincedb_path => "/dev/null"
    }
}

filter
{
	useragent
	{
		source => "ua"
		target => "ua"
	}

    mutate
    {
        remove_field => ["path", "host", "@version", "@timestamp", "ua"]
    }

	ruby
	{
		code => "event['t'] = DateTime.now.strftime('%Q')"
	}
}

output
{
	file
	{
		path => '/opt/logstash-filter-useragent/dev/bench.json'
	}
}
```

Logstash is run: ``logstash agent -w 2 -b 20 -f /opt/logstash.conf``

Query:

```sql
SELECT (CAST(MAX(t.t) AS BIGINT) - CAST(MIN(t.t) AS BIGINT)) / 1000  FROM dfs.root.`bench1.json` t
```

## Results

| Version | Run | Duration | CPU | Memory |
| ------- | --- | -------- | --- | ------ |
| 2.0.8   | logstash agent -w 2 -b 20 -f /opt/logstash.conf | 134 s | 190% | 290 MB |
| 3.0.0   | logstash agent -w 2 -b 20 -f /opt/logstash.conf | 33 s | 140% | 320 MB |
