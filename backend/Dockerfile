# Use a base image with Node.js installed
FROM node:13.12.0-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json (if available) to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the backend code into the container
COPY . .

# Expose the port that the backend server will run on
EXPOSE 5000

CMD ["npm", "start"]

