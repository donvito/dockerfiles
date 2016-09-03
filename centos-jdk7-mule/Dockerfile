FROM centos

MAINTAINER melvindave@gmail.com

RUN yum -y update
RUN yum -y install java-1.7.0-openjdk
RUN yum -y install wget

RUN mkdir /apps
RUN cd /apps

RUN wget https://repository.mulesoft.org/nexus/content/repositories/releases/org/mule/distributions/mule-standalone/3.7.0/mule-standalone-3.7.0.tar.gz

RUN tar xvzf ./mule-standalone-3.7.0.tar.gz
RUN rm ~/mule-standalone-3.7.0.tar.gz

RUN ln -s /apps/mule-standalone-3.7.0 /opt/mule

ENV JAVA_HOME /usr/lib/jvm/jre-1.7.0-openjdk

CMD [ "/opt/mule/bin/mule" ]



