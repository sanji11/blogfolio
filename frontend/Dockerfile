FROM node:current-alpine3.12

WORKDIR /usr/src/blogfolio

COPY ./package.json ./package.json
RUN npm install

COPY ./pages ./pages

ENTRYPOINT [ "/bin/sh", "-c" ,"npm start" ]
