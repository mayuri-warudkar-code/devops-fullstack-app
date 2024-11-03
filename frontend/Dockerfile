# Use an official Node.js runtime as a parent image
FROM node:14.17.0

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of your application code
COPY . .

# Expose port 3000 for the React development server
EXPOSE 3000

# Start the React application
CMD ["npm", "start"]
