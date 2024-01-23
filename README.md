
# Docker Image and Containerization 
# Wrote a Dockerfile and Created a Dockerfile in root of the project. 
# Used an official base image FROM node:14 
# Sets the working directory WORKDIR /app 
# Copied package files and install dependencies COPY package*.json ./ RUN npm install 
# Build the Docker Image
docker build -t myapp
# Run a Docker Container
docker run -p 3000:3000 -d myapp
# http://localhost:3000 on web browser to access containerized application.


