# Project Setup Instructions

## Prerequisites
- Node.js
- Python 3.10
- Docker
- AWS CLI
- kubectl
- Terraform

## Frontend Setup
cd frontend
npm install
npm start

## Backend Setup
cd backend
pip install -r requirements.txt
flask run

## Infrastructure Setup
cd setup/terraform
terraform init
terraform apply

## Kubernetes Setup
aws eks update-kubeconfig --region <region> --name <cluster-name>
kubectl apply -f k8s/

## CI/CD
GitHub Actions is used for:
- Continuous Integration (lint, test, build)
- Continuous Deployment (build, push, deploy)

