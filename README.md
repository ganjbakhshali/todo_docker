# todo_docker


## Description

MyImage is a Docker image that runs This is a Todo application built with FastAPI and SQLite. It provides a simple API for managing tasks.

## Features
- CRUD operations for tasks (Create, Read, Update, Delete)
- SQLite database backend
- Error handling for HTTP exceptions

## Requirements
- Python 3.x
- FastAPI
- SQLite3


Access the API endpoints:
* View all tasks: http://localhost:8000/tasks [GET]
* Add a new task: http://localhost:8000/tasks [POST]
* Update a task: http://localhost:8000/tasks/{id} [PUT]
* Delete a task: http://localhost:8000/tasks/{id} [DELETE]
## Usage

### Building the Docker Image

To build the Docker image, after cloning, run the following command in the terminal:

```bash
docker build -t myimage .
```

# Running the Docker Container
To run the Docker container, execute the following command:
```
docker run -d --name mycontainer -p 80:80 myimage
```
Replace mycontainer with the desired name for your container.

# Accessing the Application
Once the container is running, you can access the application by opening a web browser and navigating to http://localhost. If you're using Docker Toolbox or Docker Machine, replace localhost with the IP address of your Docker machine.
