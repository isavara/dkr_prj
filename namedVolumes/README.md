# Docker Named Volume Example: MySQL Data Persistence

This repository provides a step-by-step guide to demonstrate how to use **Docker named volumes** to persist data in a MySQL container. The setup ensures that even if the container is removed, the data remains intact.

---

## 📌 Use Case

The goal is to:
- Create a named Docker volume.
- Use it to persist MySQL database data.
- Verify that the data is retained even after the container is deleted and re-created.

---

## 🚀 Steps to Reproduce

1. **Create a Docker Named Volume**  
   Start by creating a Docker-managed volume that will store MySQL data.

2. **Run a MySQL Container with the Volume Mounted**  
   Launch a MySQL container and mount the named volume to the container’s data directory.

3. **Verify the Setup**  
   Ensure the container is running and the volume is attached correctly.

4. **Access the Database**  
   Connect to the running MySQL container using a client and create or view a database.

5. **Stop and Remove the Container**  
   Safely stop and remove the MySQL container.

6. **Recreate a New Container Using the Same Volume**  
   Start a new MySQL container using the same named volume.

7. **Verify Data Persistence**  
   Reconnect and confirm that the previously created database still exists, proving data persistence.

---

## 📘 Additional Notes

- This approach is useful for local development and testing environments.
- Docker named volumes are managed by Docker, making them portable and easier to maintain.
- No manual directory management on the host is required.

---

## ✅ Outcome

By following these steps, users can understand how Docker named volumes work and how they help in maintaining persistent data across container restarts and rebuilds.

---

## 💡 Want to Go Further?

You can extend this example by:
- Using `docker-compose` for orchestration
- Adding automatic backups for the volume
- Integrating this with an application container (e.g., a Node.js or Python app)

