FROM node:latest
LABEL maintainer="foo@bar.com"

RUN git clone https://github.com/kewashi/hpserver.git
RUN cd hpserver
RUN npm install

EXPOSE 3080

ENTRYPOINT ["node hpserver.js >& hpserver.log &"]
