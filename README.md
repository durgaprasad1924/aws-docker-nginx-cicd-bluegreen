# AWS Production CI/CD with Docker & Nginx (Blue-Green)

## Overview

This project demonstrates a production-grade DevOps setup on AWS using Docker, Nginx, CI/CD, Blue–Green deployment, and HTTPS automation.

The system supports:
- Zero-downtime deployments
- Automated CI/CD using GitHub Actions
- Blue–Green deployment strategy
- Secure HTTPS with auto-renewing SSL (Let’s Encrypt)

Live URL: https://www.durga-prasad-devops.space

## Architecture

The application follows a reverse-proxy based architecture with automated deployment and traffic switching.

![Architecture Diagram](architecture.png)

## Tech Stack

- AWS EC2 (Ubuntu)
- Docker
- Nginx (Reverse Proxy)
- GitHub Actions (CI/CD)
- Blue–Green Deployment
- Let’s Encrypt (SSL)
- Linux

## CI/CD Workflow

1. Developer pushes code to GitHub (main branch)
2. GitHub Actions pipeline is triggered
3. Application is built as a Docker image
4. New version is deployed to Green environment
5. Nginx switches traffic after verification
6. Zero downtime is maintained

## Blue–Green Deployment Strategy
- Blue environment serves live traffic
- Green environment receives new deployments
- Traffic switching is handled via Nginx upstream
- Rollback is instant by switching back to Blue

## HTTPS & Security
- HTTPS enabled using Let’s Encrypt (Certbot)
- Auto-renewal configured
- HTTP traffic redirected to HTTPS
- Secure reverse proxy using Nginx

### Author 
Durga Prasad  
DevOps Engineer  
LinkedIn: https://www.linkedin.com/in/durgaprasadpachakula/

