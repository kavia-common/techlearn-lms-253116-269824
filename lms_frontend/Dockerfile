# Use an official node image as the base
FROM node:18

# Set the working directory to the canonical project path
WORKDIR /home/kavia/workspace/code-generation/techlearn-lms-253116-269824/lms_frontend

# Copy package.json and package-lock.json first for layer caching
COPY package.json ./
COPY package-lock.json ./

# Install dependencies
RUN npm install

# Copy the rest of the app
COPY . .

# Expose the port the app runs on
EXPOSE 3000

# Start the react app
CMD ["npm", "start"]
