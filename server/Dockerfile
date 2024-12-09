
FROM node:18.20.4-alpine

WORKDIR /app

COPY package*.json ./

RUN npm install --legacy-peer-deps
RUN npm install dotenv --force

COPY . .

COPY .env .env

EXPOSE 8000

CMD ["npm", "start"]
