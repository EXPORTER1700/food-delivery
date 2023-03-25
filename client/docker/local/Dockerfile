FROM node:17-alpine3.14

WORKDIR /client

COPY ./tsconfig.json ./
COPY ./package.json ./
COPY ./package-lock.json ./
COPY ./src ./src/

RUN npm install

EXPOSE ${CLIENT_PORT}

CMD [ "npm", "run", "dev" ]