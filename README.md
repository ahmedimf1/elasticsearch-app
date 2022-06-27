# Download and Run ElasticSearch in a Docker container

### `docker network create elastic`
### `docker pull docker.elastic.co/elasticsearch/elasticsearch:7.15.2`
### `docker run --name es01-test --net elastic -p 127.0.0.1:9200:9200 -p 127.0.0.1:9300:9300 -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch:7.15.2`

# Download and Run Kibana in a Docker container

### `docker network create elastic`
### `docker pull docker.elastic.co/kibana/kibana:7.15.2`
### `docker run --name kib01-test --net elastic -p 127.0.0.1:5601:5601 -e "ELASTICSEARCH_HOSTS=http://es01-test:9200" docker.elastic.co/kibana/kibana:7.15.2`

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

