# Elasticsearch 9.x

## Setup Elasticsearch
Run the following to run elasticsearch and kibana
```bash
docker-compose up
```
to check if elasticsearch and kibana are running
Go to browser and check following links -> http://localhost:9200 and http://localhost:5601

9200 -> Rest APIs for client to interact
9300 -> internode communication
5601 -> Kibana access

## Check health
Using Kibana -> Management -> Dev Tools
```bash
GET /_cluster/health
```
or using curl
```bash
curl localhost:9200/_cluster/health
```
## Check info about nodes
```bash
GET /_nodes
```
## Get data in tabular format | v -> headers
```bash
GET /_cat/nodes?v
```
