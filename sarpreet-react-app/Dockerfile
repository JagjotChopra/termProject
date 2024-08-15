# Stage 1: Build
FROM node:20-alpine as build

# Set working directory
WORKDIR /sarpreet-react-app

# Copy package.json and package-lock.json
COPY /package*.json ./

# Install dependencies
RUN npm install

# Build the application
RUN npm run build

# Expose port 3000
EXPOSE 3000

# Start nginx
CMD ["npm", "start"]
