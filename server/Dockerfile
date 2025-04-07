FROM node:18
# RUN apk add --no-cache openssl1.1


WORKDIR /server

COPY src/ /server/src

COPY prisma/ /server/prisma

COPY package.json /server

RUN npm install

RUN npx prisma generate

