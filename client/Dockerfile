# Use the official Node.js image as the base image
FROM node:18.20.4-alpine

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json (or yarn.lock if using Yarn)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application files
COPY . .

# Expose port 3000 to access the React app
EXPOSE 3000

# Set the environment variable for the React app's start command
ENV NODE_ENV=production

# Run the app using the start command (typically npm start for React apps)
CMD ["npm", "start"]
