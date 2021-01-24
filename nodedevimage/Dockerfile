FROM node:10.23.1-alpine3.9

LABEL maintainer="rajiv@utmail.net"

RUN apk add --no-cache bash

# install items for node
RUN npm install express
RUN npm install -g nodemon

WORKDIR /home/app
USER node
ENV PORT 3000

EXPOSE 3000

ENTRYPOINT /bin/bash
