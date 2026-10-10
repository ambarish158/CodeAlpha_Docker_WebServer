# CodeAlpha Docker Web Server

## Project Overview
This project demonstrates how to deploy a web server inside a Docker container using Nginx.

It was developed as part of the CodeAlpha DevOps Internship.

## Objectives
- Understand Docker containerization.
- Build a custom Docker image.
- Deploy a web server inside a container.
- Map container ports to the host machine.
- Verify container status and HTTP responses.

## Technologies Used
- Docker Desktop
- Dockerfile
- Nginx (Alpine Linux image)
- HTML and CSS
- Windows 11

## Project Structure
```text
CodeAlpha_Docker_WebServer/
├── Dockerfile
├── index.html
└── README.md
```

## Implementation

### Build the Docker Image
```bash
docker build -t codealpha-webserver .
```

### Run the Container
```bash
docker run -d -p 8080:80 --name codealpha-webserver codealpha-webserver
```

### Check Running Containers
```bash
docker ps
```

### Test the Web Server
Open http://localhost:8080 in a browser.

Alternatively, run:
```bash
curl.exe -I http://localhost:8080
```

## Expected Result
The custom HTML webpage is served by Nginx inside a Docker container. The web server should return an HTTP 200 OK response when operating correctly.

## Learning Outcomes
- Docker image creation and container execution.
- Basic web server deployment.
- Host-to-container port mapping.
- Container verification and troubleshooting.
