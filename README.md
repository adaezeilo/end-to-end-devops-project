## Project Overview

This project demonstrates a complete end-to-end DevOps workflow by deploying a simple web application using Docker and AWS EC2.
The application is containerized, pushed to Docker Hub, and deployed on a live cloud server.

##  Technologies Used

- Docker
- AWS EC2
- Terraform
- Git & GitHub
- HTML (Basic Web App)


## Project Architecture

- Created a simple web application using HTML
- Containerized the application using Docker
- Pushed Docker image to Docker Hub
- Provisioned an EC2 instance on AWS using Terraform
- Installed Docker on EC2
- Pulled image from Docker Hub
- Ran container and exposed it on port 80

  ## Deployment Steps
1. Provision Infrastructure
Used Terraform to create:
EC2 instance
Security Group (Ports 22, 80, 443)

## Application Setup
Created a simple HTML application
3. Containerization
Dockerized the application using Nginx
Built and ran the container
4. Deployment
Deployed the container on AWS EC2
Accessed via public IP

### LIVE  APPLICATION
## Access the live app here:
http://3.84.242.193
(live app.webp)



## DOCKER  COMMANDS USED
docker build -t devops-web-app .
docker tag devops-web-app adaezeilo/devops-web-app
docker push adaezeilo/devops-web-app
docker pull adaezeilo/devops-web-app
docker run -d -p 80:80 adaezeilo/devops-web-app
(docker1.webp)

## Infrastructure (Terraform)

This project uses Terraform to provision AWS infrastructure:
- EC2 instance for hosting the application
- Security group to allow web traffic (port 80 and 5000)
Terraform configuration is located in the /terraform directory.

## Security Note

Currently, the application is served over HTTP.
Future improvement includes:
Configuring HTTPS using SSL (Let's Encrypt)
Setting up a reverse proxy (Nginx)

## AUTHOR
Precious

## WHAT I LEARNED
How to provision infrastructure using Terraform
How to containerize applications using Docker
How to deploy applications on AWS EC2
Understanding DevOps workflow from development to deployment



