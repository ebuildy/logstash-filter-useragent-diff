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

## Benchmark1: v3.0.0

=> 42 secondes

## Benchmark2: v2.0.8

=> 257.953 secondes
