# Use the official Node.js 16 image as a base
FROM node:16

# Set the working directory in the container to /app
WORKDIR /app

# Copy package.json and package-lock.json if present
COPY package*.json ./

# Install any dependencies
RUN npm install

# Copy the rest of your application code to the container
COPY . .

# Expose port 3000 for your application
EXPOSE 3000

# Command to run your application
CMD ["npm", "run", "dev"]
