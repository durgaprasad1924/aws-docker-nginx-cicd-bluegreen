# AWS Production CI/CD with Docker & Nginx (Blue-Green)

## Overview
This project demonstrates a production-style CI/CD pipeline on AWS
using Docker, Nginx, and GitHub Actions with zero-downtime deployment.

## Architecture
- GitHub Actions for CI/CD
- AWS EC2 as compute
- Docker for application packaging
- Nginx as reverse proxy
- Blue-Green deployment strategy

## Tech Stack
AWS EC2, Docker, Nginx, GitHub Actions, Linux

## Deployment Strategy
Blue-Green deployment is used to avoid downtime during releases.

