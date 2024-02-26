FROM docker.elastic.co/logstash/logstash-oss:8.10.0
COPY logstash-output-kusto-2.0.5-java.gem /tmp/logstash-output-kusto-2.0.5-java.gem
RUN rm -f /usr/share/logstash/pipeline/logstash.conf && \
  bin/logstash-plugin install /tmp/logstash-output-kusto-2.0.5-java.gem