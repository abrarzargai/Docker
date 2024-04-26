# Simple Dockerized Node.js App

This is a basic example of how to Dockerize a Node.js application (using Dockerfile).

## Prerequisites

Before you begin, ensure you have the Docker installed on your local machine:

- [Docker](https://www.docker.com/get-started)

## Getting Started

To get a local copy up and running follow these simple steps:

### Installation

1. Clone the repository
   ```sh
   git clone repository_name
   ```
2. Navigate into the project directory
   ```sh
   cd project-directory
   cd simple-docker-node
   ```

### Building the Docker Image

3. Build the Docker image
   ```sh
   docker build -t my-node-app .
   ```
   `This command builds a Docker image 🖼️ for your Node.js app based on the instructions in your Dockerfile. The -t flag gives the image a name (my-node-app), and the . specifies the current directory as the build context`

### Running the Docker Container

4. Run the Docker container

   ```sh
   docker run -p 8080:8080 my-node-app

   ```

   `This command creates and starts a Docker container 📦 based on the my-node-app image. The -p flag maps port 8080 of the host machine to port 8080 of the container, allowing you to access your Node.js app`

5. Open your web browser and go to:

   ```sh
   http://localhost:8080
   ```
