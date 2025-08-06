# Task 2 - DevOps Internship @ Elevete Labs

## 📅 Day 2 Task

### ✅ Task Title: CI/CD Pipeline for Node.js App using Jenkins & Docker

---

## 🛠️ Tech Stack Used:
- Node.js
- Git & GitHub
- Docker
- Jenkins (Installed using Docker)

---

## 📂 Files Included:
- index.js - Basic Node.js server
- package.json - Defines dependencies
- Dockerfile - Container image setup
- Jenkinsfile - CI/CD pipeline configuration
- README.md - Project documentation

---

## 🔄 Pipeline Stages (Defined in `Jenkinsfile`):
1. **Checkout** - Clone the GitHub repository
2. **Install Dependencies** - Run `npm install`
3. **Build Docker Image** - Create a Docker image using the Dockerfile
4. **Run Docker Container** - Deploy the app inside a container

---

## ⚙️ Jenkins Setup:
- Jenkins was installed inside a Docker container
- Required plugins installed
- Jenkins pipeline created using GitHub repo:  
  🔗 https://github.com/Saitejabatti/Nodejenkinsdemo

---

## 🚀 How to Run Manually:

# Clone the repository
git clone https://github.com/Saitejabatti/Nodejenkinsdemo.git
cd Nodejenkinsdemo

# Install Node.js dependencies
npm install

# Run app locally
node index.js

# OR build and run with Docker
docker build -t nodejenkinsdemo .
docker run -p 3000:3000 nodejenkinsdemo

📸 Output:
✅ Successful Jenkins Pipeline Execution:
Code checked out from GitHub

npm install completed successfully

Docker image built: nodejenkinsdemo

Container started successfully using the image

The Jenkins console log confirms each step completed without error.
