# Movie Picture Pipeline Project

## Overview
This project implements a CI/CD pipeline for a movie catalog application using GitHub Actions. The application consists of a frontend built with React (TypeScript) and a backend API built with Flask (Python).

## Architecture
- Frontend: React (TypeScript)
- Backend: Flask (Python)
- CI/CD: GitHub Actions
- Containerization: Docker
- Deployment: Kubernetes (AWS EKS)

## CI/CD Pipeline

### Continuous Integration
- Triggered on pull requests
- Runs lint checks
- Executes unit tests
- Builds application

### Continuous Deployment
- Triggered on push to main
- Builds Docker images
- Tags images using Git SHA
- Pushes images to AWS ECR
- Deploys to Kubernetes cluster

## Project Structure
