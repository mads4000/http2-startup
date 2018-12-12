FROM docker.elastic.co/elasticsearch/elasticsearch-oss:6.3.2

WORKDIR /usr/share/elasticsearch

RUN /usr/share/elasticsearch/bin/elasticsearch-plugin install analysis-icu

COPY elasticsearch.yml /usr/share/elasticsearch/config
