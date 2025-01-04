FROM node:18-alpine

WORKDIR /frontend

COPY package*.json ./

RUN npm cache clean --force && \
    npm install ajv@6.12.6 && \
    npm install ajv-keywords@3.5.2 && \
    npm install schema-utils@3.1.1 && \
    npm install

COPY . .

EXPOSE 3000

CMD ["npm", "start"]