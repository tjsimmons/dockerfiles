FROM node:latest
LABEL maintainer="foo@bar.com"

WORKDIR /hpserver

RUN git clone https://github.com/kewashi/hpserver.git
RUN npm install

EXPOSE 3080

ENTRYPOINT ["node hpserver.js >& hpserver.log &"]
