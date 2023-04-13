FROM maven:3.6.3-jdk-8 AS builder
WORKDIR /build

RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git \
    && cd boxfuse-sample-java-war-hello \
    && mvn clean \
    && mvn package -DskipTests