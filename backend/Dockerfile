FROM node:18-alpine

WORKDIR /usr/apps/backend

COPY package.json ./
COPY yarn.lock ./

RUN yarn install --frozen-lockfile --production

COPY . ./

RUN yarn build

ENTRYPOINT yarn start
