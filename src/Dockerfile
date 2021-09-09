FROM node:alpine

LABEL maintainer "eric.muellenbach@yncrea.fr"

ADD app.js .

WORKDIR /src/app
COPY ./ /src/app

RUN npm install express
RUN npm install morgan
RUN npm install mongoose

ENTRYPOINT [ "node", "app.js" ]
