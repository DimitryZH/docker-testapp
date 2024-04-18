## Overview

This project involves Dockerizing a simple PHP web application named "testapp" to facilitate testing in various scenarios such as setting up CI/CD pipelines, Dockerizing applications, and testing Kubernetes manifests. The application displays a webpage containing basic information and the server's IP address.

### Components

1. **index.php**: This file contains the PHP code for the web application. It retrieves the server's IP address using `$_SERVER['SERVER_ADDR']` and displays it on a webpage along with some basic information about the application.

2. **Dockerfile**: The Dockerfile defines the environment and dependencies required to run the PHP web application. It starts with the base image `amazonlinux:1`, updates the package manager (`yum`), installs Apache HTTP Server (`httpd`), and installs PHP. Then, it copies the `index.php` file into the appropriate directory for serving web content. Finally, it specifies the command to start the HTTP server and exposes port 80 for incoming HTTP connections.

### Purpose

The purpose of the "testapp" is to provide a lightweight application that can be easily deployed and tested in different environments and scenarios. By Dockerizing the application, it becomes portable and can be run consistently across various platforms. The ability to display the server's IP address adds value, especially in scenarios where multiple instances of the application are deployed, and knowing the server's IP is necessary for troubleshooting or configuration purposes.

### Usage

Once Dockerized, the "testapp" Docker image can be deployed to any Docker-compatible environment, such as local development machines, CI/CD pipelines, or Kubernetes clusters. Users can pull the Docker image from a registry or build it locally using the provided Dockerfile. Once the Docker container is running, accessing the application via a web browser will display the webpage with the server's IP address and other information.

Overall, this project provides a useful tool for testing and experimenting with different deployment and orchestration solutions, while also serving as a simple example of containerizing a PHP web application with Docker.

### Result

![php-testapp](https://github.com/DimitryZH/docker-testapp/assets/146372946/51b28e70-3da6-4b42-b314-70adb122e45d)

