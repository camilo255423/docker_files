FROM ubuntu:18.04
RUN apt-get update
RUN apt-get install -y iputils-ping 
RUN apt-get install -y net-tools
RUN apt-get install -y default-jdk
RUN apt-get install -y scala
RUN apt-get install -y openssh-server openssh-client
RUN apt-get install -y vim
RUN wget https://www-eu.apache.org/dist/spark/spark-2.4.1/spark-2.4.1-bin-hadoop2.7.tgz
RUN tar xvf spark-2.4.1-bin-hadoop2.7.tgz
RUN mv spark-2.4.1-bin-hadoop2.7 spark
RUN mv spark /usr/local/
ENV PATH="/usr/local/spark/bin:${PATH}"
EXPOSE 80 443 8080 4040

