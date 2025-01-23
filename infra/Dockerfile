# Use official Node.js image as the base image
FROM node:16


# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy the package.json and package-lock.json (if exists) from the app directory
COPY ../app/package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application files from the app directory
COPY ../app ./

# Expose the port that the app runs on
EXPOSE 3000

# Command to run the application
CMD ["npm", "start"]

