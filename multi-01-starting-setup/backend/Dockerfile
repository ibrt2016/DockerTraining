FROM node

WORKDIR /app

COPY package.json /app

RUN npm install

COPY . .

ARG DEFAULT_PORT=80

ENV PORT=${DEFAULT_PORT}

ENV MONGODB_USERNAME=root

ENV MONGODB_PASSWORD=secret

EXPOSE ${PORT}

CMD [ "npm", "start" ]