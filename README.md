# Project 13: Build Docker Image and Push to Amazon ECR

## Objective
Build a Docker image for a web application and push it to Amazon Elastic Container Registry (ECR).

## Tools Used
- Ubuntu Linux
- Docker
- AWS CLI
- Amazon ECR
- Nginx Alpine

## Project Files
- Dockerfile
- index.html
- README.md

## AWS Configuration
- Region: eu-west-1
- ECR Repository: project13-app
- Image Tag: latest

## Implementation
1. Created a simple HTML web application.
2. Created a Dockerfile using Nginx Alpine.
3. Built the Docker image locally.
4. Logged in to Amazon ECR.
5. Tagged the image with the ECR repository URI.
6. Pushed the image to Amazon ECR.
7. Verified the image using AWS CLI.

## ECR Repository URI
590507089733.dkr.ecr.eu-west-1.amazonaws.com/project13-app

## Verification
Command:
aws ecr describe-images --repository-name project13-app --region eu-west-1 --image-ids imageTag=latest

## Result
Successfully built and pushed the Docker image to Amazon ECR.
