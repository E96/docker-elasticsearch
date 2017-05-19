FROM docker.elastic.co/elasticsearch/elasticsearch:5.3.0
RUN bin/elasticsearch-plugin install http://dl.bintray.com/content/imotov/elasticsearch-plugins/org/elasticsearch/elasticsearch-analysis-morphology/5.3.0/elasticsearch-analysis-morphology-5.3.0.zip
ADD config/license.json data/license.json
#RUN /usr/bin/curl -XPUT -u elastic:changeme 'http://localhost:9200/_xpack/license' -d @data/license.json