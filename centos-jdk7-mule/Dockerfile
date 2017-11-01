FROM melvindave/centos7-jdk7:v1

MAINTAINER melvindave@gmail.com

RUN yum -y update
RUN yum -y install java-1.7.0-openjdk
RUN yum -y install wget

RUN wget https://repository.mulesoft.org/nexus/content/repositories/releases/org/mule/distributions/mule-standalone/3.7.0/mule-standalone-3.7.0.tar.gz

RUN cd /opt && tar xvzf ~/mule-standalone-3.5.0.tar.gz
RUN rm ~/mule-standalone-3.5.0.tar.gz
RUN ln -s /opt/mule-standalone-3.5.0 /opt/mule 

CMD [ "/opt/mule/bin/mule" ]

