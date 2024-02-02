
FROM node:14.15.4-alpine3.12

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

COPY src .

EXPOSE 3000

CMD [ "node", "index.js" ]