# 🐳 Docker Activities:
---
**This file documents all the Docker activities for week 1, code blocks for the Dockerfile and all docker commands used.**
---

```markdown
# 🐳 Docker Activities – Hello World App

## 📌 Task
Build, run, and push a basic Docker image.

---

## 🛠️ Steps

### 1. Write a simple “Hello World” application
You can use either **Python** or **Node.js**.  
Here’s an example in **Python**:

```python
# app.py
print("Hello, World from Docker!")
```

---

### 2. Create a Dockerfile
```dockerfile
# Use official Python image as base
FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Copy application file
COPY app.py .

# Run the application
CMD ["python", "app.py"]
```

### Requirements.txt
``` flask==2.3.2
requests==2.31.0
```

---

### 3. Build the image
Run the following command in the same directory as your `Dockerfile`:

```bash
docker build -t hello-world-app .
```

---

### 4. Run the container locally
```bash
docker run --rm hello-world-app
```

Expected output:
```
Hello, World from Docker!
```

---

### 5. Push the image to Docker Hub
1. **Login to Docker Hub**:
   ```bash
   docker login
   ```

2. **Tag the image**:
   ```bash
   docker tag hello-world-app <your-dockerhub-username>/hello-world-app:latest
   ```

3. **Push the image**:
   ```bash
   docker push <your-dockerhub-username>/hello-world-app:latest
   ```

---

## 📂 Submission Checklist
- ✔️ **Dockerfile**  
- ✔️ **Screenshot of running container**  
- ✔️ **Docker Hub image link**  

Example Docker Hub link:  
https://hub.docker.com/repository/docker/elyon1/mydockerapp/general

---
```
