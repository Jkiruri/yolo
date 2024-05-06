# STAGE 1
# Use the Node base image with Alpine Linux for building
FROM node:alpine as build

# Set the working directory inside the container
WORKDIR /code

# Copy package.json and package-lock.json to the container
COPY package.json package.json
COPY package-lock.json package-lock.json

# Install dependencies
RUN npm install --production

# Copy the rest of the application files to the container
COPY . .

# Build the application
RUN npm run build

# STAGE 2
# Use the Nginx base image with Alpine Linux for production
FROM nginx:1.22-alpine as prod

# Copy the build output from the first stage to the Nginx web server directory
COPY --from=build /code/build /usr/share/nginx/html

# Expose port 3000 for incoming connections
EXPOSE 3000

# Command to start the Nginx server
CMD ["nginx", "-g", "daemon off;"]