FROM docker.elastic.co/beats/filebeat-oss:6.4.2

COPY  filebeat.yml /usr/share/filebeat/

USER root
RUN chown root:filebeat /usr/share/filebeat/filebeat.yml
RUN chmod go-w /usr/share/filebeat/filebeat.yml
USER filebeat

RUN filebeat modules list
RUN filebeat modules enable apache2
