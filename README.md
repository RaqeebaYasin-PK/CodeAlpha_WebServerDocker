# Task 4 — Web Server Using Docker  
**CodeAlpha DevOps Internship Project**

## Project Overview

This project completes **Task 4: Web Server using Docker**, focusing on building, containerizing, and running a web server inside a Docker container. The main objectives were to:

- Learn Docker containerization basics  
- Deploy and manage a web server inside Docker containers  
- Understand container lifecycle and commands  
- Monitor container health and troubleshoot issues  
- Explore container-based app deployment best practices  

---

## Tech Stack

| Technology | Version |
|------------|---------|
| Node.js    | v18 (Docker base image) |
| Express.js | Latest |
| Docker     | Latest |

---

## Project Structure

server.js # Node.js web server
package.json # Dependencies and scripts
package-lock.json # Exact dependency versions
Dockerfile # Docker container build instructions



---

## Prerequisites

- Docker (Engine or Desktop)  
- Git  

Clone the repository:

git clone https://github.com/RaqeebaYasin-PK/CodeAlpha_WebServerDocker.git
cd CodeAlpha_WebServerDocker



---

## Running Locally (Without Docker)

Install dependencies:

npm install

powershell


Start the server:

node server.js



Open your browser:

http://localhost:3000



---

## Docker Usage

### Build Docker Image

docker build -t webserver-advanced .

shell


### Run Docker Container

docker run -p 3000:3000 webserver-advanced



Access the app:

http://localhost:3000



---

## API Endpoints

| Route  | Description                  |
|--------|------------------------------|
| `/`    | Serves static web page       |
| `/api` | Returns JSON API response    |

---

## Docker Concepts Covered

- **Images** – Layered blueprint containing app + environment  
- **Containers** – Isolated runtime instances  
- **Port Mapping** – Exposing container services to host machine  
- **Build Context & Caching** – Efficient iterative builds  

---

## Learning Outcomes

By completing this project, I gained practical experience in:

- Building and running a web server  
- Containerizing applications with Docker  
- Mapping ports and networking containers  
- Creating reproducible, environment-independent deployments  

---

## Future Enhancements

- Publish Docker image to Docker Hub  
- Add automated CI/CD pipeline (GitHub Actions)  
- Include unit tests for API endpoints  
- Add monitoring for container health  

---

## Author

**Raqeeba Yasin**  
GitHub: [https://github.com/RaqeebaYasin-PK](https://github.com/RaqeebaYasin-PK)
