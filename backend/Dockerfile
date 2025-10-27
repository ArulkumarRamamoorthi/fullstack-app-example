# Use official Node.js image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install --production

# Copy rest of the backend source code
COPY . .

# Expose backend port (change if your server runs on different port)
EXPOSE 5000

# Start the backend server
CMD ["node", "server.js"]
