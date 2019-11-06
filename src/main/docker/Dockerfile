FROM openjdk:8-jdk-alpine

RUN apk update && apk upgrade

RUN mkdir -p /usr/local/webapi-example

ADD  @project.build.finalName@.jar /usr/local/webapi-example/

ADD run.sh run.sh
 
RUN chmod +x run.sh
 
CMD ./run.sh