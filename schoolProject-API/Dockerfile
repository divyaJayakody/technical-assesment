# FROM node:12-alpine as build-step
# WORKDIR /app
# COPY package.json /app
# RUN npm install
# COPY . /app
# CMD ["node", "server.js"]

FROM node:15-alpine as build-step
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
COPY package.json /usr/src/app
RUN npm install
COPY . /usr/src/app
EXPOSE 3000
CMD ["npm","start"]