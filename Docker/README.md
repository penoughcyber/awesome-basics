# What is Docker?

Docker is a tool that allows you to create, deploy, and run applications inside containers. Containers are like mini virtual machines, but they are much lighter and more efficient. With Docker, you can package your application and all its dependencies into a single container, making it easy to move between different environments (e.g., from your laptop to the cloud).

<p align="center">
<img src="./Resources/docker-icon.png" alt="Docker Icon" width="300">
</p>

Further, We need to learn about how docker came. Actually, Docker was introduced in 2013 by a company called Docker, Inc. The idea was to make it easier to develop and run applications consistently across different computing environments. And, You know what this was a game-changer in the DevOps world!

- [Features and Charactistics of Docker](#Features-and-Characteristics-of-Docker)
- [Traditional Deployment vs Docker Deployment](#Traditional-Deployment-vs-Docker-Deployment)
- [Architecture of Docker and its use case](#Architecture-of-Docker-and-its-use-case)
- [Why use Docker?](#Why-use-Docker)
- [Docker Installation](#Docker-Installation)
  - [Ubuntu](#)
  - [Windows](#)
  - [MacOS](#)

# Features and Characteristics of Docker

# Traditional Deployment vs Docker Deployment

# Architecture of Docker and its use case

# Why use Docker?

Here are a few reasons why Docker has become a must-have tool for developers and IT professionals:

* **Consistency:** Docker ensures your application runs the same way whether where it’s deployed on a PC, a test environment, or a production server, Docker containers make sure that consistency should be there. This eliminates the “but it worked on my machine” syndrome and reduces the time spent on debugging environment-related issues.
* **Isolation and Security:** Containers isolate applications from each other and the underlying system. This means that each container operates independently, it prevents conflicts, and enhances security. For example, if one container experiences a security breach or failure, it won’t affect other containers running on the same host.
* **Efficiency and Speed:** Docker is lightweight, Unlike virtual machines, which include a full OS for each instance. Here, containers share the host system kernel. This makes them faster to start and overhead on the system resources. As a result, you can run many more containers on the same hardware compared to VM.
* **Scalability and Flexibility:** If we need to handle more traffic Docker can make it easy to spin up additional containers to distribute the load. Docker integrates seamlessly with orchestration tools like Kubernetes, making it simple to manage containerized applications at scale. This means you can dynamically adjust resources to meet demand without downtime.
* **Portability Across Platform:** Docker containers can run on any system that supports Docker, be it Linux, Windows, or macOS. This portability ensures that applications can move easily between development, testing, and production environments, simplifying workflows and reducing the chances of compatibility issues.

Lastly, Docker has transformed the software development lifecycle by providing a consistent, efficient, and scalable environment for building, sharing, and running applications. Whether you're a developer, system admin, or IT professional, Docker's impact is undeniable.
If you haven't explored Docker yet, now's the time! Dive in, experiment, and see how it can simplify and accelerate your projects.

# Docker Installation
How to Install docker in your `Ubuntu 22.04` System.

## Step 1: Install Docker on Ubuntu 22.04

1. Update the package list:

   ```shell
   sudo apt-get update
   ```
2. Install Docker:

   ```shell
   sudo apt-get install docker.io
   ```
3. Check the docker version:

   ```shell
   sudo docker --version
   ```
   
4. You can start the Docker service and configure it to run on startup by entering the following commands:

   ```shell
   sudo systemctl start docker
   sudo systemctl enable docker
   ```
5. Verify the status of the docker service:

   ```shell
   sudo systemctl status docker
   ```