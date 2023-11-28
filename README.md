# deploy-web-appplication-to-kubernetes
This repository contains the necessary deployment and service manifests to create a Kubernetes pod running a web application using a custom Docker image hosted on my personal Docker Hub repository.

## Start Minikube

```minikube start```

## Set Docker environment to Minikube:

```eval $(minikube docker-env)```

## Apply Deployment

```kubectl apply -f deployment.yaml```

## Apply Service

```kubectl apply -f service.yaml```

## Get the Minikube IP and port to access application

```minikube service my-note-app-service --url```