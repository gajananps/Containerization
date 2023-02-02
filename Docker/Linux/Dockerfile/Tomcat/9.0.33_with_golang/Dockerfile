FROM tomcat:9.0.33-jdk8

RUN apt-get update -y

RUN cd /tmp

RUN wget https://golang.org/dl/go1.10.3.linux-amd64.tar.gz

RUN tar -xvf go1.10.3.linux-amd64.tar.gz

RUN rm -rf go1.10.3.linux-amd64.tar.gz

RUN mv go /usr/local

ENV PATH=$PATH:/usr/local/go/bin

RUN apt-get install -y go-bindata
