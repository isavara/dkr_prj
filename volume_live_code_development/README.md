# Docker Volumes - Bind mount
# 🚀 Dockerizing a Node.js Application

This guide provides step-by-step instructions to Dockerize your Node.js application and expose it on **port 5000**.

---

## 🧱 Step 1: Create a Dockerfile

Start by creating a file named `Dockerfile` in the root of your project.

---

## 🔹 Step 2: Choose a Base Image

Use an official Node.js base image (node:18) from Docker Hub that matches your Node.js version.

---

## 🔹 Step 3: Set the Working Directory

Specify a working directory inside the container where the application will reside.

---

## 🔹 Step 4: Copy Dependency Files

Copy `package.json` and `package-lock.json` into the container. This helps in caching dependency installation.

---

## 🔹 Step 5: Install Dependencies

Run the command to install all required Node.js packages.

---

## 🔹 Step 6: Copy Application Source Code

Copy all the source files from your local directory into the working directory inside the container.

---

## 🔹 Step 7: Expose the Application Port

Expose **port 5000**, or whatever port your application listens on.

---

## 🔹 Step 8: Define the Startup Command

Specify the command that should run when the container starts. Usually, it would start your Node.js app.

---

## 🐳 Building and Running the Docker Image

1. Build the Docker image using the Dockerfile.
2. Run the container, mapping **port 5000** of the container to your host.

---

## ✅ Example Usage

While actual code is not included here, follow the instructions above to:
- Write your Dockerfile
- Build the image
- Run the container

For help or questions, feel free to raise an issue or reach out.

---

