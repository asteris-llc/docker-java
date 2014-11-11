FROM centos:centos7

MAINTAINER Steven Borrelli <steve@aster.is>

ENV JAVA_VERSION 8u25
ENV JAVA_VERSION_MINOR b17

RUN yum -y install wget
RUN wget --quiet --no-check-certificate --no-cookies --header "Cookie: oraclelicense=accept-securebackup-cookie" http://download.oracle.com/otn-pub/java/jdk/$JAVA_VERSION-$JAVA_VERSION_MINOR/jdk-$JAVA_VERSION-linux-x64.rpm

RUN rpm -ivh jdk-$JAVA_VERSION-linux-x64.rpm  && \
    rm -f jdk-$JAVA_VERSION-linux-x64.rpm
