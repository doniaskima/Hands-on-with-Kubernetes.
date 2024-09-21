# Hands-on-with-Kubernetes

This repository contains a practical guide for getting started with Kubernetes. It includes example configurations and hands-on exercises to help you deploy, manage, and scale applications in a Kubernetes cluster.

## Getting Started

### Prerequisites

Before you begin, make sure you have the following installed:

- [Kubernetes CLI (kubectl)](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
- A Kubernetes cluster (can be a local cluster like [Minikube](https://minikube.sigs.k8s.io/docs/start/) or a cloud provider such as GKE, AKS, or EKS)
- [Docker](https://www.docker.com/) for containerization

### Quick Start

1. Clone the repository:

    ```bash
    git clone https://github.com/doniaskima/Hands-on-with-Kubernetes..git
    cd hands-on-with-kubernetes
    ```

2. Deploy a sample MongoDB application:

    ```bash
    kubectl apply -f mongodb-deployment.yaml
    ```

3. Check the status of the deployment:

    ```bash
    kubectl get deployments
    kubectl get pods
    ```

4. Expose the MongoDB service:

    ```bash
    kubectl apply -f mongodb-service.yaml
    ```

5. Verify that the MongoDB service is running:

    ```bash
    kubectl get services
    ```

### Key Concepts

- **Deployments**: Manage and scale your application with Kubernetes deployments.
- **Services**: Expose your applications internally or externally within the cluster.
- **Secrets**: Store sensitive data such as passwords and access tokens securely.

## Learn More

For more information, refer to the official [Kubernetes Documentation](https://kubernetes.io/docs/).

 