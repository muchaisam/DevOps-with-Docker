FROM ubuntu:18.04
FROM openjdk:8

WORKDIR /usr/app
EXPOSE 8080

RUN apt-get update
RUN apt-get install -y git

RUN git clone https://github.com/docker-hy/spring-example-project.githttps://github.com/docker-hy/spring-example-project.git

WORKDIR /src/spring-example-project

RUN chmod +x mvnw

RUN ./mnvw package

CMD [ "/bin/sh", "-c", "java -jar ./target/docker-example-1.1.3.jar" ]