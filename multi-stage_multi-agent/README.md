# Multi-Stage Multi-Agent Jenkins Pipeline

## 📌 Project Overview
This project demonstrates a **Jenkins Declarative Pipeline** implementing both **multi-stage** and **multi-agent** configurations.  
It automates the process of verifying environment versions for both **Maven** (Java backend) and **Node.js** (frontend) in isolated Docker containers.

## 🚀 Features
- **Multi-Stage Build**: Separate stages for backend (Maven) and frontend (Node.js).
- **Multi-Agent Execution**: Each stage runs on a different Docker image.
- **Docker Integration**: Builds run inside lightweight, containerized environments.
- **CI/CD Automation**: Fully integrated with GitHub repository and deployed on AWS EC2.
- **Permission Configuration**: Jenkins user granted Docker permissions for seamless container execution.

## 🛠️ Tech Stack
- **Jenkins** (Declarative Pipeline)
- **Docker**
- **AWS EC2**
- **GitHub**
- **Maven** (`maven:3.8.1-adoptopenjdk-11`)
- **Node.js** (`node:16-alpine`)

## 📂 Pipeline Stages
1. **Backend Stage**  
   - Runs in a `maven:3.8.1-adoptopenjdk-11` Docker container.
   - Checks Maven installation and version.

2. **Frontend Stage**  
   - Runs in a `node:16-alpine` Docker container.
   - Checks Node.js installation and version.

