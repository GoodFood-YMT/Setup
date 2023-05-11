# Setup
Setup instructions for the project

## Prerequisite

- Docker (or Docker Desktop)
- Kubernetes (or integrated with Docker Desktop)
- Helm

## Instructions

Create Kubernetes namespace
`kubectl create namespace goodfood`

Install Nginx Ingress to Kubernetes
`helm upgrade --install ingress-nginx ingress-nginx 
  --repo https://kubernetes.github.io/ingress-nginx 
  --namespace ingress-nginx --create-namespace`

You can now setup micro-services one by one.
