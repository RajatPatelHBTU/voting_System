FROM node:20-slim
WORKDIR /app

# Copy package files
COPY package*.json ./
RUN npm install

# Copy source code
COPY . .

# Build the TypeScript project
RUN npm run build

EXPOSE 3000
CMD ["npm", "start"]
