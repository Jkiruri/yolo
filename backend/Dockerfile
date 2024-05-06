# Use the official Node.js image with Alpine Linux 3.18 as the base image
FROM node:alpine3.18 

# Set the working directory inside the container
WORKDIR /

# Copy package.json and package-lock.json files to the container
COPY package*.json ./

# Install dependencies

RUN npm install

# Copy the rest of the application code to the container
COPY . .

# Expose port 5000 for incoming connections
EXPOSE 5000

# Command to run the Node.js application
CMD ["npm", "start"]
