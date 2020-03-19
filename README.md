# elk

Dockercompose v3 sample to start Elasticsearch/Kibana for local playground.
Prerequisite: docker & docker-compose available locally.

## Usage

Start everything
``` sh
docker-compose up -d
```

Stop everything
``` sh
docker-compose down
```

## Browsing

Elaticsearch started on http://localhost:9200
Kibana started on http://localhost:5601

[Kibana](https://www.elastic.co/guide/en/kibana/current/getting-started.html) & [Elasticsearch](https://www.elastic.co/guide/en/elasticsearch/reference/current/index.html) documentation

## Notes

* takes a couple of seconds to startup, URLs won't be available until then.

To get a startup status, check
``` sh
docker-compose logs -f
```
* data is not persisted. Mount a docxcker volume to persist any test data

## See also

[docker-compose sample from docs](https://www.elastic.co/guide/en/elastic-stack-get-started/current/get-started-docker.html#run-stack-docker) - requires older docker-compose version (v2), is a bit more complex.
