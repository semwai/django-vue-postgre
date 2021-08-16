# syntax=docker/dockerfile:1
FROM node:14

WORKDIR /usr/src/code

COPY package*.json ./

RUN npm install -g cross-env

RUN npm install

COPY . .

EXPOSE 8080
