# Use the official Node.js image for version 14.17.0
FROM node:14.17.0

# Set the working directory
WORKDIR /app

# Copy the package.json and package-lock.json files
COPY package*.json ./

# Install the dependencies
RUN npm install

# Copy the source code
COPY . .

# Expose the application's port
EXPOSE 3000

# Run the application
CMD ["npm", "start"]

