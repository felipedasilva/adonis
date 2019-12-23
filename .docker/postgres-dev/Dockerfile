FROM postgres:10

RUN apt-get update && apt-get -y install wget build-essential postgresql-server-dev-10
RUN apt-get install unzip

RUN wget https://github.com/HypoPG/hypopg/archive/master.zip
RUN unzip master.zip
WORKDIR /hypopg-master 
RUN make
RUN make install