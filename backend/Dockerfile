# Backend Dockerfile for CineWorld DevOps project
FROM node:18-alpine

# Set working directory inside container
WORKDIR /app

# Copy package files first
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the source code
COPY . .

# Expose port and start app
EXPOSE 3000
CMD ["node", "server.js"]
