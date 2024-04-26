# Use the Node.js 18 Alpine base image
FROM node:18-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json files into the container
COPY package*.json ./

# Install dependencies using npm ci (faster and more reliable for production)
RUN npm ci

# Copy the rest of the application files into the container
COPY . .

# Expose port 8080 to the outside world
EXPOSE 8080

# Command to start the application
CMD ["npm","start"]
