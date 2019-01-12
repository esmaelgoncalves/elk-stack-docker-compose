# elk-stack-docker-compose

**elk-stack-docker-compose** is a sample how to install ELK stack using docker.
This stack is composed with de thw following applications:
+ elasticsearch 6.5
+ kibana 6.5
+ logstash 6.5

## Quick Start:
+ Fork this repo
+ Clone the repo: `git clone https://github.com/esmaelgoncalves/elk-stack-docker-compose.git`
+ Download de Zip file.

## Pre-Requiriments
+ Docker - [Docker](https://www.docker.com/get-started)
+ Filebeat - [FileBeat](https://www.elastic.co/products/beats/filebeat)

## Startup
Choose one of the two options betweeen:
**elasticsearch-single-kibana-docker-compose.yml** to setup a single instance of elasticsearch, kibana and logstash
or
**elasticsearch-multiple-kibana-docker-compose.yml** to setup a cluster of elasticsearch with two instances, single instance of kibana and single instance of logstash

1. docker-compose filename.yml up (to start with dettached option use -d option)
2. elasticsearch will be available at port 9200 (use http:localhost:9200 to verify)
```
{
  "name" : "ObOgHm2",
  "cluster_name" : "docker-cluster",
  "cluster_uuid" : "7tZJtmsqQZK8WHIv1sdqOg",
  "version" : {
    "number" : "6.5.4",
    "build_flavor" : "default",
    "build_type" : "tar",
    "build_hash" : "d2ef93d",
    "build_date" : "2018-12-17T21:17:40.758843Z",
    "build_snapshot" : false,
    "lucene_version" : "7.5.0",
    "minimum_wire_compatibility_version" : "5.6.0",
    "minimum_index_compatibility_version" : "5.0.0"
  },
  "tagline" : "You Know, for Search"
}
````
3. kibana will be available at port 5601