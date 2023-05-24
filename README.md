# Prometheus-grafana-compose

This is a docker-compose file to deploy prometheus and grafana in your server. 
Prometheus is a monitoring system and Grafana is a visualization tool for Prometheus. 
With this compose file, you can easily deploy them in your server.

Also, the prometheus.yml file is a sample configuration file for prometheus. 
It has some basic configurations for connecting a Service Discovery - Nacos, and the services registered in Nacos will expose a http API /actuator/prometheus to provide monitoring information, then prometheus can collect the information of all microservices automatically. 
You can modify it to fit your needs.

## Prerequisites
- Docker and docker compose installed in your server

## Getting started

```
docker create network prometheus
docker-compose up -d
```
