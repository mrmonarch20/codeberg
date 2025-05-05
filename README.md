
# Codeberg Repository - Flask Docker Application

This repository contains a simple Flask application that returns the current timestamp and the visitor's IP address. The application is containerized using Docker for easy deployment.

---

## Features

- **Timestamp Display**: Returns the current timestamp in the `Asia/Kolkata` timezone.
- **Visitor IP**: Displays the visitor's IP address.
- **Dockerized**: Containerized using Docker for ease of deployment and portability.

---

## Prerequisites

Ensure the following are installed and configured on your system:
- **Docker CLI**: Installed and available on the `PATH`.
- **Docker Daemon**: Running on the host machine.

---

## Getting Started

### 1. Build the Docker Image

Use the following command to build the Docker image:

```bash
docker build -t flask-app .
```

### 2. Run the Docker Container

Run the following command to start the container and map port 5000:

```bash
docker run --rm -p 5000:5000 flask-app
```

### 3. Access the Application

Open your browser or use curl to access the application at http://localhost:5000.
You should see a JSON response similar to the example below:

```JSON
{
    "timestamp": "2025-05-05T12:34:56+05:30",
    "ip": "127.0.0.1"
}
```


### Files in the Project

 --->Dockerfile: Defines the Docker image for the Flask application.

 --->app.py: The Flask application code.

 --->requirements.txt: Lists the Python dependencies for the application.


### Stopping the Container

To stop the container:

Press Ctrl+C if the container is running interactively.

Alternatively, use the following command:

```bash
docker stop <container-id>
```

### Cleanup

After stopping the container, you can remove it using:

```bash
docker rm <container-id>
```


### Repository Details
Repository URL: https://github.com/mrmonarch20/codeberg
Owner: mrmonarch20
Primary Language: Python
Feel free to modify this README file to include additional details or features as the project evolves!

```Code

Let me know if you’d like me to help you upload this README file to your repository!
```
