FROM node:18-alpine

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

RUN npm test

RUN npm run build

EXPOSE 3002

CMD ["node", "start-server.js"]
