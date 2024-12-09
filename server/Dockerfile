
FROM node:18.20.4-alpine

WORKDIR /app

COPY package*.json ./

RUN npm install --legacy-peer-deps
RUN npm install dotenv --force

COPY . .

COPY .env .env

# Expose the port the backend will run on
EXPOSE 8000

# Set the environment variable for production


# Start the server using npm (since your command is npm start)
CMD ["npm", "start"]
