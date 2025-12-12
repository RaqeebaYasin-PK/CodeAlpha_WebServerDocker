# CodeAlpha Task 4 — Web Server using Docker

This project demonstrates how to deploy a simple Node.js web server inside a Docker container.

## Features
- Simple Node.js + Express web server
- Dockerfile for containerization
- Run the app inside a Docker container
- Exposes port 3000

## How to Run

### 1. Build Docker Image
docker build -t webserver-image .

### 2. Run Container
docker run -p 3000:3000 webserver-image

### 3. Open in browser
http://localhost:3000

