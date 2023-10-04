FROM node:18.16.1-alpine3.18

RUN mkdir -p /app
WORKDIR /app

COPY package*.json ./

#install nodemon globally 
RUN npm install nodemon -g

#install packages
RUN npm install

#app code goes here
COPY . .

EXPOSE 5000

CMD ["npx", "nodemon", "app.js"]

