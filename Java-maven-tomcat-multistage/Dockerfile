FROM ubuntu:latest as builder
RUN apt-get update && \
     apt-get install -y openjdk-8-jdk wget unzip

 ARG MAVEN_VERSION=3.9.6
 RUN wget https://dlcdn.apache.org/maven/maven-3/3.9.6/binaries/apache-maven-3.9.6-bin.tar.gz && \
     tar -zxvf apache-maven-${MAVEN_VERSION}-bin.tar.gz && \
    rm apache-maven-${MAVEN_VERSION}-bin.tar.gz && \
    mv apache-maven-${MAVEN_VERSION} /usr/lib/maven
