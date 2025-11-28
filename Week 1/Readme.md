# Welcome to Week 1 of 12 Weeks DevOps Foundation Mastery Project.
---
## Week 1: Introduction to DevOps Foundations and Toolchain Setup
---
# **📘 Week 1 – DevOps Foundations & Toolchain Setup**

**Project 0 – Toolchain Setup and Cloud Introduction**

---

## **🎯 Objective**

The goal of Week 1 is to **set up your complete DevOps workstation** and gain hands-on familiarity with foundational DevOps tools.
By the end of this week, you should have working knowledge of:

* Cloud basics (AWS)
* Version control (Git + GitHub)
* Infrastructure-as-Code basics
* Containers and Docker
* Networking & security fundamentals
* System setup and CLI tooling

This prepares you for deeper DevOps tasks in the coming weeks.

---

# **📂 Week 1 Tasks & Deliverables**

---

## **1. 🖥️ System & Tooling Setup (Local Machine)**

### **Task:**

Install and configure essential DevOps tools required for the 12-week program.

### **Tools to Install**

* Visual Studio Code
* Git
* Docker Desktop
* AWS CLI
* GitHub CLI or GitLab CLI (optional)
* Postman
* cURL

### **Deliverables**

Upload the following:

* ✔️ Screenshot of each installed tool
* ✔️ Output of:

```
git --version
aws --version
docker --version
```

---

## **2. 🔧 Version Control – Git & GitHub**

### **Task:**

Create a Git repository and practice core Git workflow operations.

### **Steps**

1. Initialize a new Git repository

   ```bash
   git init
   ```
2. Create a README.md describing your DevOps journey
3. Create a new branch

   ```bash
   git checkout -b feature/setup
   ```
4. Add and commit files

   ```bash
   git add .
   git commit -m "Initial setup"
   ```
5. Merge `feature/setup` into `main`
6. Push repository to GitHub
7. Create a Pull Request and merge it

### **Deliverables**

* ✔️ GitHub repository link
* ✔️ Screenshot of merged Pull Request
* ✔️ Markdown file containing all Git commands used

---

## **3. ☁️ AWS Cloud Foundations**

### **Task:**

Set up AWS and explore the core services.

### **Activities**

* Create an **IAM user** with programmatic access
* Configure AWS CLI:

  ```bash
  aws configure
  ```
* Launch a **Free-tier EC2 instance**
* Create an **S3 bucket**
* View EC2 metrics in **CloudWatch**
* Explore your default VPC and identify:

  * VPC ID
  * Subnet IDs
  * Route tables

### **Deliverables**

* ✔️ Screenshot of IAM user (no access keys revealed)
* ✔️ EC2 instance screenshot
* ✔️ S3 bucket screenshot
* ✔️ Output of:

  ```bash
  aws s3 ls
  ```

---

## **4. 🐳 Docker & Containers**

### **Task:**

Build, run, and push a basic Docker image.

### **Steps**

1. Create a simple “Hello World” app (Python or Node)
2. Write a Dockerfile
3. Build image

   ```bash
   docker build -t mydockerapp .
   ```
4. Run the container

   ```bash
   docker run mydockerapp
   ```
5. Push image to Docker Hub

### **Deliverables**

* ✔️ Dockerfile
* ✔️ Screenshot of container running
* ✔️ Link to Docker Hub image

---

## **5. 📊 Monitoring & Logging**

### **Task:**

Explore AWS CloudWatch logs and metrics.

### **Activities**

* Check EC2 CPU Utilization
* View default EC2 system logs
* Identify existing alarms

### **Deliverables**

* ✔️ Screenshot of CloudWatch metrics
* ✔️ Screenshot of CloudWatch logs

---

## **6. 🌐 Networking & Security Basics**

### **Task**

Create a document explaining:

* Public Subnet
* Private Subnet
* Security Groups
* DNS record types supported by Route 53
* How SSH key pairs work

### **Deliverable**

* ✔️ A markdown file named **`networking_basics.md`**

---

## **7. 📝 Documentation**

### **Task:**

Document the entire Week 1 work in a single README.

### **Content Checklist**

* ✔️ Tools installed
* ✔️ AWS tasks completed
* ✔️ Git workflow summary
* ✔️ Terraform steps (if any)
* ✔️ Docker steps
* ✔️ CI/CD setup (if done)
* ✔️ Screenshots
* ✔️ Challenges encountered
* ✔️ Key learnings
