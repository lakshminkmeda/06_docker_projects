Simple Hello World app for Docker testing

1. The hello world app uses nodejs and listens on port 3000. The output is a simple "Hello Node" message.

Useful commands:


docker build -t myapp:v1 .
docker run -d -p 3000:3000 myapp:v1


# Hello Node.js Docker Application

A simple Node.js application created for Docker testing and learning purposes.

The application starts a web server on port **3000** and returns a simple response:

```text
Hello Node
```

---

## Project Overview

This project demonstrates:

* Building a Docker image for a Node.js application
* Running a containerized application
* Exposing application ports
* Testing Docker container networking

---

## Application Details

* Runtime: Node.js
* Listening Port: 3000
* Response: "Hello Node"

Example:

```text
http://localhost:3000
```

Returns:

```text
Hello Node
```

---

## Build the Docker Image

```bash
docker build -t hello-node:v1 .
```

---

## Run the Container

```bash
docker run -d -p 3000:3000 hello-node:v1
```

### Port Mapping

```text
Host Port      Container Port
3000      ->   3000
```

---

## Access the Application

Open a browser and navigate to:

```text
http://localhost:3000
```

## Verify the Container

List running containers:

```bash
docker ps
```

View container logs:

```bash
docker logs <container-id>
```

---

## Stop the Container

```bash
docker stop <container-id>
```

---

## Learning Objectives

This project helps demonstrate:

* Docker fundamentals
* Container image creation
* Node.js application deployment
* Port exposure and mapping
* Container lifecycle management

---

## Technologies Used

* Node.js
* Docker
* JavaScript
