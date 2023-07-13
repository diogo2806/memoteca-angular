FROM node:14

WORKDIR /app

COPY package*.json ./

RUN npm install -g json-server

EXPOSE 3000

CMD ["npm", "start"]
