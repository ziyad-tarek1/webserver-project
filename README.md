# Webserver Project

## Description

The **Webserver Project** is a simple web application setup designed to demonstrate the use of Docker for deploying multiple web services. This project utilizes Docker Compose to orchestrate three separate instances of the Apache HTTP Server, each serving its own static website content.

## Project Structure
[ziad@localhost webserver-project]$ tree
.
├── docker-compose.yaml
├── nginx.conf
├── web1
│   └── index.html
├── web2
│   └── index.html
└── web3
    └── index.html

    
- **docker-compose.yaml**: Defines the services, networks, and volumes for the Docker containers.
- **nginx.conf**: Copy it to /etc/nginx/nginx.conf
- **web1, web2, web3**: Directories containing static HTML files for each web service.

## Features

- **Multi-Service Architecture**: Run multiple web services in parallel using Docker.
- **Port Mapping**: Each web service is accessible on a different port:
  - **Web Service 1**: `http://localhost:8081`
  - **Web Service 2**: `http://localhost:8082`
  - **Web Service 3**: `http://localhost:8083`
- **Volume Mounting**: Local directories are mounted into the containers for live updates.

## Getting Started

To get started with the Webserver Project, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/ziyad-tarek1/webserver-project.git
   ```
   
2. **Navigate to the Project Directory:**
  ```bash
cd webserver-project
```
3. **Run Docker compose up
``` bash
docker-compose up
```
 
