# Frontend Dockerfile for React

# Use official Node.js image
FROM node:14-slim

# Set working directory
WORKDIR /frontend

# Copy package.json and install dependencies
COPY package.json /frontend/
RUN npm install

# Copy frontend files
COPY . /frontend/

# Expose React app port
EXPOSE 3000

# Command to run the frontend
CMD ["npm", "start"]
