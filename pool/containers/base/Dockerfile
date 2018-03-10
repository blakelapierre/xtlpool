FROM ubuntu

RUN apt-get update
RUN apt-get install -y wget

RUN wget https://github.com/stellitecoin/Stellite/releases/download/1.2.1.0/linux-x64-1.2.1.0.zip
RUN unzip linux-x64-1.2.1.0.zip -d coin
RUN mv linux-x64-1.2.1.0 coin


CMD cd coin/bin && ./stellited --data-dir /daemon-data