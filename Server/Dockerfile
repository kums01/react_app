# Using the official Node.js image as the base image version
FROM node:14-alpine

# Setting the working directory inside the container 
WORKDIR /usr/src/app

# Copying package.json and the package-lock.json to the working DIR
COPY package*-json ./

# Installing application dependencies
RUN npm install

# Copying rest all files to working DIR (for ex. nodemon and express packages)
COPY . . 

# Exposing the port (Same as my node backend application)
EXPOSE 5000

# Starting the server (dev refers to nodemon Dev package which basically starts node server.js)
CMD [ "npm", "run", "dev"]

