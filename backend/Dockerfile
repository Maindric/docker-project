FROM node:latest

RUN mkdir -p /src/app

WORKDIR /src/app

COPY . /src/app

RUN yarn install

RUN yarn global add nodemon

EXPOSE 3000

ARG DB_CONNECTION_STRING

ENV DB_CONNECTION_STRING $DB_CONNECTION_STRING

CMD [ "./startup.sh" ]