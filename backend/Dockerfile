# Use a base image with Node.js installed
FROM node:14

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the backend code into the container
COPY . .

# Expose the port that the backend server will run on
EXPOSE 5000

# Define the command to run the backend server
CMD ["node", "server.js"]
