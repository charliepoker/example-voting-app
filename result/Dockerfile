# Use Node.js LTS image based on Alpine Linux
FROM node:18-alpine

# Create and set the working dirctory
WORKDIR /app

# Copy package.json and package-lock.json (if available)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Set the environment variable for the port
ENV PORT 80

# Expose port 80
EXPOSE 80

# Command to run the application
CMD ["node", "server.js"]
