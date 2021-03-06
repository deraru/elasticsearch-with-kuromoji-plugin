# elasticsearch-with-kuromoji-plugin

[deraru/elasticsearch-with-kuromoji-plugin - Docker Hub](https://hub.docker.com/r/deraru/elasticsearch-with-kuromoji-plugin/)

## Sample wercker.yml

```
services:
  - id: deraru/elasticsearch-with-kuromoji-plugin
build:
  steps:
    - script:
      name: Set ELASTIC_SEARCH environment variables
      code: |
        export ELASTIC_SEARCH_HOST=${ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9200_TCP_ADDR}
        export ELASTIC_SEARCH_PORT=${ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9200_TCP_PORT}
```

## Environment variables on Wercker

- ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT
- ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9200_TCP
- ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9200_TCP_ADDR
- ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9200_TCP_PORT
- ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9200_TCP_PROTO
- ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9300_TCP
- ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9300_TCP_ADDR
- ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9300_TCP_PORT
- ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9300_TCP_PROTO

### Sample values

```
ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT="tcp://192.168.100.8:9200"
ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9200_TCP="tcp://192.168.100.8:9200"
ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9200_TCP_ADDR="192.168.100.8"
ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9200_TCP_PORT="9200"
ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9200_TCP_PROTO="tcp"
ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9300_TCP="tcp://192.168.100.8:9300"
ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9300_TCP_ADDR="192.168.100.8"
ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9300_TCP_PORT="9300"
ELASTICSEARCH_WITH_KUROMOJI_PLUGIN_PORT_9300_TCP_PROTO="tcp"
```
