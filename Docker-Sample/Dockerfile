# Use a specific Node.js version
FROM node:16
# Verify node and npm installation
RUN node -v && npm -v
# Install nodemon globally using npm
RUN npm install -g nodemon
# Set the working directory
WORKDIR /home/app
# Copy the current directory contents into the container at /home/app
COPY . .
# Install dependencies
RUN npm install
# Expose the port the app runs on
EXPOSE 3000
# Run the application with nodemon
CMD ["nodemon", "index.js"]