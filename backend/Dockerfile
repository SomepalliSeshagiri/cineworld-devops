# Backend Dockerfile for CineWorld DevOps project
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package files from backend folder
COPY backend/package*.json ./

# Verify package.json is copied correctly
RUN echo "Files in /app:" && ls -l && cat package.json

# Install dependencies
RUN npm install --omit=dev

# Copy the rest of backend source code
COPY backend/ .

# Expose app port
EXPOSE 3000

# Start Node.js app
CMD ["node", "server.js"]
