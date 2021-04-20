# FROM node:14.15.5
FROM node:14-slim

WORKDIR /usr/src/app

COPY ./package.json ./
COPY ./yarn.lock ./

# RUN yarn
RUN yarn install

COPY . .

EXPOSE 5000

CMD [ "yarn", "start" ]