# 1️⃣  Base Image
FROM node:18

# 2️⃣  Working Directory
WORKDIR /app

# 3️⃣  Copy Dependency Files
COPY package*.json ./

# 4️⃣  Install Dependencies
RUN npm install

# 5️⃣  Copy Remaining Application Files
COPY . .

# 6️⃣  Expose App Port
EXPOSE 3000

# 7️⃣  Default Command to Run the App
CMD ["node", "server.js"]
