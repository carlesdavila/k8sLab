# k8sLab

Kubernetes Lab

## Overview

This project is a sample application designed to demonstrate the deployment of a .NET application in a Kubernetes environment. It includes a Dockerfile for containerizing the application and a Kubernetes Pod configuration file for deployment.

## Project Structure

- **`src/SampleApi`**: Contains the source code for the .NET application.
- **`pods/pod.yml`**: Kubernetes Pod configuration file for deploying the application.
- **`Dockerfile`**: Used to build the Docker image for the application.

## Prerequisites

- Docker installed on your machine.
- Kubernetes cluster set up (e.g., Minikube, AKS, etc.).
- `kubectl` CLI installed and configured.

## Build and Run

### Build the Docker Image

Run the following command from the root directory of the project (where the `.sln` file is located):

```bash
docker build -f src/SampleApi/Dockerfile -t carlesdavila/k8slab:1.0 .