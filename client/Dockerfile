# This will be more similar to Server's Dockerfile as this is a simple React Application
FROM node:14-alpine

WORKDIR  /usr/src/app

COPY package.json  .

RUN npm install

COPY . .

EXPOSE 3000

CMD [ "npm", "start"]
#ignore