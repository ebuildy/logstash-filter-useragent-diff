# logstash-filter-useragent-diff

Difference between logstash filter useragent 2.0.8 (UA parser) and 2.1.0 with Bitwalker Java parser

## Methode

I run logstash with ua_sample.json as file input, 2 times:
- 1 => filter useragent v2.0.8 (current)
- 2 => filter useragent v2.1.0 (java)

Logstash output to output.json file, then I use Apache Drill to do SQL queries against json files.

## Links

| Link | Title |
| ---- | ----- |
| [/logstash.conf](https://github.com/ebuildy/logstash-filter-useragent-diff/blob/master/logstash.conf) | Logstash configuration |
| [/sample.json](https://github.com/ebuildy/logstash-filter-useragent-diff/blob/master/sample.json) | user agents sample (input) |
| [/output1.json](https://github.com/ebuildy/logstash-filter-useragent-diff/blob/master/output1.json) | output v2.0.8 |
| [/output2.json](https://github.com/ebuildy/logstash-filter-useragent-diff/blob/master/output2.json) | output v2.1.0 |
| [/results_name_os.md](https://github.com/ebuildy/logstash-filter-useragent-diff/blob/master/results_name_os.md) | Results OS names |
| [/name_diff.md](https://github.com/ebuildy/logstash-filter-useragent-diff/blob/master/name_diff.md) | browser name differences |
| [/os_diff.md](https://github.com/ebuildy/logstash-filter-useragent-diff/blob/master/os_diff.md) | OS differences |
| []() | |
| [/benchmark.md](https://github.com/ebuildy/logstash-filter-useragent-diff/blob/master/benchmark.md) | Performance benchmark |

## Format

**v2.1.0 Mozilla/5.0 (Windows NT 6.1; WOW64; rv:44.0) Gecko/20100101 Firefox/44.0**

```json
{
"name":"Firefox",
"fullname":"Firefox 44",
"vendor":"Mozilla Foundation",
"type":"Browser",
"major":"44",
"minor":"0",
"version":"44.0",
"os":"Windows 7",
"os_vendor":"Microsoft Corporation",
"os_name":"Windows",
"os_type":"Computer"
}
```

**v2.0.8 Mozilla/5.0 (Windows NT 6.1; WOW64; rv:44.0) Gecko/20100101 Firefox/44.0**

```json
{
"name":"Firefox",
"os":"Windows 7",
"os_name":"Windows 7",
"device":"Other",
"major":"44",
"minor":"0"
}

```
