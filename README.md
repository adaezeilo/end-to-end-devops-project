Project Overview

This project demonstrates a complete end-to-end DevOps workflow by deploying a simple web application using Docker and AWS EC2.
The application is containerized, pushed to Docker Hub, and deployed on a live cloud server.

TECHNOLOGIES USED
Docker 
AWS EC2 
Git & GitHub
HTML (Basic Web App)

PROJECT  ARCHITECTURE
Created a simple web application (HTML)
Containerized the app using Docker
Pushed Docker image to Docker Hub
Provisioned an EC2 instance on AWS
Installed Docker on EC2
Pulled image from Docker Hub
Ran container and exposed it on port 80

LIVE  APPLICATION
Access the live app here:
http://3.84.242.193

DOCKER  COMMANDS USED
docker build -t devops-web-app .
docker tag devops-web-app adaezeilo/devops-web-app
docker push adaezeilo/devops-web-app
docker pull adaezeilo/devops-web-app
docker run -d -p 80:80 adaezeilo/devops-web-app

FUTURE IMPROVEMENTS
Implement CI/CD pipeline using GitHub Actions
Use Terraform for infrastructure automation
Add custom domain and HTTPS (SSL)
Automate deployment process

AUTHOR
Precious

WHAT I LEARNED
How to containerize applications using Docker
How to deploy applications on AWS EC2
How to manage Docker images with Docker Hub
Basics of cloud deployment and DevOps workflow

