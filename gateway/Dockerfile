FROM node:lts-alpine

RUN npm install -g npm
RUN mkdir -p /var/www/gateway

WORKDIR /var/www/gateway
ADD . /var/www/gateway

RUN npm install

CMD npm run build && npm run start:prod
