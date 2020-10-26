FROM node:current-alpine3.12

WORKDIR /usr/src/blogfolio

COPY ./package.json ./package.json
RUN npm install

COPY ./public ./public
COPY ./styles ./styles
COPY ./pages ./pages
COPY ./components ./components

RUN npm run build

ENTRYPOINT [ "/bin/sh", "-c" ,"npm start" ]
