FROM ubuntu

RUN apt-get update
RUN apt-get install -y wget unzip

RUN wget https://github.com/stellitecoin/Stellite/releases/download/1.2.2.0/linux-x64-1.2.2.0.zip
RUN unzip linux-x64-1.2.2.0.zip -d coin


CMD cd coin/bin && ./stellited --data-dir /daemon-data