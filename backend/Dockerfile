FROM node:latest

WORKDIR /backend

COPY package.json .

RUN npm install -g nodemon

RUN npm install

COPY . .

EXPOSE 80

CMD [ "nodemon", "app.js" ]