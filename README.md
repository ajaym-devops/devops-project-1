# DevOps Project 1 – Node.js CI/CD Pipeline

This is my first end-to-end DevOps project where I built a CI/CD pipeline for a Node.js application.

The goal of this project was to understand how code moves from a developer machine to a live server automatically.

Instead of manually building and deploying every time, the whole process now happens automatically after `git push`.

---

## What this project does

- Runs a simple Node.js app using Express
- Containerized using Docker
- Source code stored in GitHub
- GitHub Actions builds and deploys automatically
- Docker image pushed to Docker Hub
- EC2 server pulls latest image and runs container
- App becomes live on browser automatically after every push

---

## Tech Used

- Node.js
- Express
- Docker
- GitHub
- GitHub Actions
- Docker Hub
- AWS EC2
- Linux / Ubuntu

---

## CI/CD Flow

The deployment flow looks like this:

Developer writes code locally

↓  

git push

↓  

GitHub Actions starts automatically

↓  

Docker image gets built

↓  

Image pushed to Docker Hub

↓  

EC2 server pulls latest image

↓  

Old container removed

↓  

New container starts

↓  

Updated app goes live

---

## Run locally

Clone repo:

```bash
git clone <your-repo-url>
cd devops-project-1


---

## What I learned

This project helped me understand:

- how Docker images and containers work
- how GitHub Actions automates CI/CD
- how Docker Hub is used as a container registry
- how to deploy containers on AWS EC2
- how to debug deployment issues like:
  - port mapping issues
  - Docker login failures
  - port already allocated errors
  - SSH connection issues

The biggest takeaway for me was understanding how a simple `git push` can trigger the full deployment pipeline automatically.
