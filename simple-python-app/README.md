# Simple Python exercise
# Dockerized Python Application (Flask)

This project demonstrates how to containerize a simple Python web application and run it using Docker on port 5000.

## Prerequisites

- Python application file (e.g., `app.py`)
- Dependency list file (`requirements.txt`)
- Docker installed on your system

## Steps to Dockerize and Run

1. **Create a Dockerfile**  
   Write a Dockerfile that:
   - Uses a lightweight Python base image
   - Sets a working directory
   - Copies the `requirements.txt` and installs dependencies
   - Copies your Python application code
   - Exposes port 5000
   - Defines a command to run the application

2. **Build the Docker Image**  
   From the directory containing the Dockerfile, run the build command to create your Docker image.  

3. **Run the Docker Container**  
Use the following command to start a container from the built image and map it to port 5000 on your host:

4. **Access the Application**  
Once the container is running, open your browser and visit:

## Notes

- Ensure that your Python application listens on host `0.0.0.0` and port `5000` to work correctly inside Docker.
- If you make changes to your code, rebuild the image before re-running the container.



