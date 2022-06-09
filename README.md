# ELK-for-beginners
This is an easy exercise for beginners in the  Dockers and ELK's world. 

## Elasticsearch, Logstash, Kibana (ELK) Docker image

This is a basic ELK stack in Docker image provides a convenient centralised log server and log management web interface, by packaging Elasticsearch, Logstash, and Kibana.


## Description
Once we set up Docker, we will deploy a container running Elasticsearch, Kibana, and Logstash in the same system. 
The docker-compose.yml file help to run both the Docker image and containers based on the described configuration.

## Steps
1. Install Docker. Start by installing and setting up Docker on a system.  (https://docs.docker.com/desktop/windows/install/)
2. Install Docker Compose. We will use docker-compose to deploy our ELK stack. (https://docs.docker.com/compose/install/)
3. Clone the repository and start the containers by using Docker-compose.
4. Inside de clone repository run in a terminal or command prompt the following command: 
    - Validate the version, we need 2.0 or superior 
    ```
     docker compose version
    ```
    - To start the cluster, run docker-compose: 
    ```
     docker-compose up -d
     ```
   This docker-compose.yml file generates a three-node secure Elasticsearch cluster with authentication and network encryption enabled, as well as a Kibana instance.
   
5. Review at  docker application the exists of three images and containers. 
- docker.elastic.co/elasticsearch/elasticsearch:8.1.0
- docker.elastic.co/logstash/logstash:8.1.0
- docker.elastic.co/kibana/kibana:8.1.0
- httpd:latest
6. Check if it’s working at:
>http://localhost:9200 – Elasticsearch
>http://localhost:5044 – Logstash
>http://localhost:5601 – Kibana web
>http://localhost:8090 – Httpd 
   
