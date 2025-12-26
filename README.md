# Task 4 — Web Server Using Docker  
**CodeAlpha DevOps Internship Project**

## Project Objective

This project completes **Task 4: Web Server Using Docker**, focused on building, containerizing, and running a web server inside a Docker container. The goal was also to understand Docker fundamentals such as images, containers, port mapping, and container lifecycle.

## Tech Stack

| Technology | Version |
|------------|---------|
| Node.js    | v18 (Docker base image) |
| Express.js | Latest |
| Docker     | Latest |

---

## Project Structure

├── server.js
├── package.json
├── package-lock.json
└── Dockerfile

yaml
Copy code

---

## Getting Started

### Prerequisites

Install:
- Docker (Engine or Docker Desktop)
- Git

Clone the repository:

```bash
git clone https://github.com/RaqeebaYasin-PK/CodeAlpha_WebServerDocker.git
cd CodeAlpha_WebServerDocker
Running Locally (without Docker)
Install dependencies:

bash
Copy code
npm install
Run the server:

bash
Copy code
node server.js
Visit in browser:

arduino
Copy code
http://localhost:3000
Docker Usage
Build Docker Image
bash
Copy code
docker build -t webserver-advanced .
Run Docker Container
bash
Copy code
docker run -p 3000:3000 webserver-advanced
You can access the app in the browser:

arduino
Copy code
http://localhost:3000
Endpoints
Route	Description
/	Serves static web page
/api	Returns JSON API response

Docker Concepts Covered
Images – Layered blueprint of application + environment

Containers – Isolated runtime instances

Port Mapping – Exposing container ports to host

Build Context & Caching – Faster iterative builds

Learning Outcomes
This project helped me understand:

How to build and run a web server

Basics of Docker images and containers

Port mapping and container networking

Creating reproducible container deployments

Future Enhancements
Publish image on Docker Hub

Add automated CI/CD pipeline

Add unit tests for API endpoints

Author
Raqeeba Yasin
GitHub: https://github.com/RaqeebaYasin-PK
