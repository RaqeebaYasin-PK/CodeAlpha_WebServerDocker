# Task 4 — Web Server Using Docker  
**CodeAlpha DevOps Internship**

## Project Overview

This project completes **Task 4: Web Server using Docker** as part of the CodeAlpha DevOps Internship. The goal was to build a lightweight web server, containerize it using Docker, understand container lifecycles, and deploy it consistently across environments.

## Features

- Node.js powered backend and static frontend
- REST API endpoint
- Docker containerization for environment‑independent execution
- Demonstrates Docker build, run, and port mapping

## Tech Stack

| Technology | Version |
|------------|---------|
| Node.js    | 18 (Docker base image) |
| Express.js | Latest |
| Docker     | Latest |

## Getting Started

### Prerequisites

Install the following on your local machine:

- Docker (Docker Desktop or Engine)
- Git

Clone the repository:


git clone https://github.com/RaqeebaYasin-PK/CodeAlpha_WebServerDocker.git
cd CodeAlpha_WebServerDocker
Running Locally (without Docker)

Install dependencies:

npm install


Start the server:

node server.js


Open in browser:

http://localhost:3000

##Docker Usage
Build the Docker Image
docker build -t webserver‑advanced .

Run the Docker Container
docker run -p 3000:3000 webserver‑advanced


Container will serve the app on:

http://localhost:3000


##What it Does

Dockerfile uses node:18 as base image

Copies application source

Installs dependencies

Exposes port 3000

Runs server inside container

##Key Concepts Learned

Images: Layered blueprint containing application and runtime

Containers: Isolated execution environment

Port Mapping: Exposes container services to host

Build Context: How Docker copies and caches layers 
Docker Documentation

Example Endpoints

/ — Main web page

/api — JSON response (demo/test)

##Future Enhancements

Add test cases (e.g., using Jest)

Publish the Docker image to Docker Hub

Add GitHub Actions CI workflow

##Author

Raqeeba Yasin
GitHub: https://github.com/RaqeebaYasin-PK

DevOps / Full‑Stack Enthusiast
