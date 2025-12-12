Task 4: Web Server Using Docker (CodeAlpha DevOps Internship)

As part of the CodeAlpha DevOps Internship, I completed Task 4: Web Server Using Docker, which focuses on understanding containerization, application deployment, and platform-independent runtime environments using Docker. This task allowed me to build a production-style web server, package it into a Docker container, and run it consistently across systems.

Project Overview

The objective of this task was to:
Build a lightweight web server
Containerize the application using Docker
Run the server inside an isolated container
Understand the Docker lifecycle: image creation, container execution, port mapping, and file system structure
Apply practical DevOps workflows to ensure environment consistency and reproducibility

I implemented the project using Node.js and Express to create both a static webpage and a REST API endpoint, providing a more advanced and realistic application setup.

Technical Implementation
1. Building the Web Server
I developed a Node.js application consisting of:
A static HTML frontend served from the /public directory
A backend Express API returning JSON data
A clean and responsive interface to demonstrate real-world server behavior
The application exposes two key routes:

/ – Serves the HTML page

/api – Returns JSON response for API testing

This combination simulates a typical frontend-backend architecture used in production.

2. Containerizing the Application with Docker
Dockerfile Implementation
A production-ready Dockerfile was created to:
Define the base image (node:18)
Set up the working directory
Install dependencies
Copy the application source code
Expose port 3000

Configure the container startup command (node server.js)

This ensures that anyone running the container will get the exact same environment, regardless of their OS or machine configuration.

Building the Docker Image
docker build -t webserver-advanced .


This generated a reusable Docker image containing the full application code and runtime.

Running the Container
docker run -p 3000:3000 webserver-advanced
Port mapping (-p 3000:3000) allows external access to the container, enabling users to open the application on:
http://localhost:3000

Both frontend and API routes successfully run inside Docker, proving full containerization.

3. Understanding Docker Concepts

During the implementation, I gained hands-on experience with:

Images
Layered blueprints containing application code, dependencies, and environment configuration.
Containers
Isolated runtime instances of images that execute the application in a controlled sandbox.

Port Mapping

Forwarding container ports to host ports for external accessibility.
Build Context
Understanding how Docker copies code and manages layers for faster rebuilds.
Application Packaging
Ensuring the application runs identically across environments.
These concepts are foundational to DevOps, modern software delivery, and cloud-native deployment.

4. Outcome and Learning Impact

Completing this task strengthened my practical skills in:
Docker fundamentals
Application containerization
Working with web servers
Isolating application environments
Understanding deployment workflows
Running production-like setups locally

This hands-on experience aligns directly with DevOps practices used in CI/CD pipelines, microservices, cloud deployment, and scalable distributed systems.

Conclusion

Task 4 allowed me to design, containerize, and deploy a functional web server entirely inside Docker. The project demonstrates practical DevOps skills and showcases my ability to work with real-world container workflows. This experience builds a strong foundation for more advanced topics such as Kubernetes, CI/CD pipelines, and cloud-native application delivery.
