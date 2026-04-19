# CI/CD Pipeline

This project uses GitHub Actions to automate the development workflow.

## Continous Integration

- Runs on pull requests to main
- Lints frontend code using ESLint
- Runs frontend tests
- Builds Docker image

## Continous Deployment

- Runs on push to main - Builds Docker imange - Tags image using Git SHA
- Pushes image to AWS ECR
- Deploys application to kubernetes cluster

## Deployment flow

Developer -> GitHub -> CI -> Docker Build -> ECR -> Kubernetes
