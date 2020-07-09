FROM node:4-alpine

ENV NODE_ENV=development
ENV PORT=8080

RUN apk update && apk add make

RUN npm install -g phantomjs-prebuilt
RUN npm install -g casperjs

RUN mkdir -p /usr/src/app

COPY . /usr/src/app

WORKDIR /usr/src/app

CMD /usr/local/bin/npm start
