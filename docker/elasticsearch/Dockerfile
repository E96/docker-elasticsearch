FROM docker.elastic.co/elasticsearch/elasticsearch:5.3.0
RUN bin/elasticsearch-plugin install http://dl.bintray.com/content/imotov/elasticsearch-plugins/org/elasticsearch/elasticsearch-analysis-morphology/5.3.0/elasticsearch-analysis-morphology-5.3.0.zip
RUN bin/elasticsearch-plugin install analysis-icu
RUN  mv /usr/share/elasticsearch/plugins/x-pack /usr/share/elasticsearch/plugins/.removing-x-pack && \
     mv /usr/share/elasticsearch/plugins/.removing-x-pack /usr/share/elasticsearch/plugins/x-pack && \
     /usr/share/elasticsearch/bin/elasticsearch-plugin remove x-pack