FROM ubuntu:14.04

RUN apt-get update && apt-get install -y git build-essential redis-server libboost1.55-all-dev nodejs-dev nodejs-legacy npm cmake libssl-dev

RUN git clone https://github.com/blakelapierre/xtlpool

RUN cd xtlpool/xtlpool && npm update

EXPOSE 8117
EXPOSE 9999

ADD config.json /xtlpool/xtlpool/config.json

CMD cd xtlpool/xtlpool && node init.js