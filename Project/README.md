
# 🚀 Azure Web App Deployment using GitHub Actions

This repository demonstrates a CI/CD workflow to deploy a Dockerized Spring Boot Java application to **Microsoft Azure App Service** using **GitHub Actions**.

🔗 **GitHub Repo**: [Celebal_Project](https://github.com/vanshtarar4/Celebal_Project)  
🎥 **Showcase Video**: [Google Drive Demo](<YOUR-GOOGLE-DRIVE-LINK-HERE>)

---

## 📘 Project Description

As part of my internship at **Celebal Technologies**, I implemented an automated CI/CD pipeline to streamline software deployment for a customer-facing web application of a fictional pharmaceutical company. The goal was to ensure faster, seamless updates using **Azure Web App** and **GitHub Actions**.

This project highlights:
- Containerization of a Spring Boot application
- Integration of GitHub Actions for CI/CD
- Deployment to Azure with automated workflows

---

## 🧩 Business Problem Statement

A leading pharmaceutical company needs a modern deployment strategy to:
- Regularly update their product-related content
- Provide reliable, scalable hosting
- Automate deployment using GitHub Actions and Azure services

---

## ✅ Prerequisites

- A valid **Azure account**
- Dockerized **Spring Boot Java application**
- GitHub repository with application source code

---

## 🏗️ High-Level Architecture

```mermaid
graph TD;
    A[GitHub Repository] -->|Push Code| B[GitHub Actions Workflow];
    B --> C[Build Docker Image];
    C --> D[Push to GitHub Container Registry];
    D --> E[Azure Web App];
    E --> F[Pull Docker Image];
    F --> G[Deploy to App Service];
