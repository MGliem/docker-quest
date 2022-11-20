FROM node:lts-alpine
RUN mkdir /app
WORKDIR /app
COPY package*.json ./
COPY yarn.lock ./
COPY tsconfig*.json ./
RUN yarn install
COPY index.html ./
COPY vite.config.ts ./
COPY src src
COPY public public

CMD yarn build
