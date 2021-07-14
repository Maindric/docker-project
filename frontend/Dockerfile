FROM node:latest

RUN mkdir -p /src/app

WORKDIR /src/app

COPY . /src/app

RUN yarn install

RUN yarn global add nodemon

EXPOSE 3000

# ARG BACKEND_URL

# ENV BACKEND_URL $BACKEND_URL

CMD [ "npm", "start" ]