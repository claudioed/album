# Dockerfile for config microservice
FROM java:8
MAINTAINER Claudio de Oliveira<claudioed.oliveira@gmail.com>
VOLUME /tmp
ADD config-server-micro-1.0-SNAPSHOT.jar config-server-micro.jar
RUN bash -c 'touch /config-server-micro.jar'
EXPOSE 8001
ENTRYPOINT ["java","-Dspring.profiles.active=docker","-jar","/config-server-micro.jar"]