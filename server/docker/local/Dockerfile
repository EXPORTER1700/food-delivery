FROM node:17-alpine3.14

WORKDIR /server

COPY ./tsconfig.json ./
COPY ./tsconfig.build.json ./
COPY ./package.json ./
COPY ./package-lock.json ./
COPY ./src ./src/

RUN npm install

EXPOSE ${SERVER_PORT}

CMD [ "npm", "run", "start:dev" ]