# Dockerfile

# Step 1: Use a Node.js image to build the app
FROM node

# Set working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package.json .

# Install dependencies
RUN npm install

# Copy the rest of the app’s source code
COPY . .

# Build the app
RUN npm run build

# Expose port 5173
EXPOSE 5174

# Start the program
CMD ["npm", "run", "dev"]