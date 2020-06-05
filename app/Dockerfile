FROM node:latest

EXPOSE 5000

RUN mkdir -p /app

WORKDIR /usr/src/app

COPY package.json ./

RUN npm install && npm cache clean --force

COPY . .

CMD ["node", "app.js"]
