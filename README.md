# Firefly III on Kubernetes

## Overview

This project demonstrates the deployment of Firefly III, a personal finance management application, on a Kubernetes cluster. The deployment is managed using ArgoCD, a popular continuous delivery tool for Kubernetes.

## Project Structure

The project is designed to run Firefly III within a Kubernetes environment, utilizing the following components:

- **ConfigMap**: Manages configuration data for Firefly III.
- **Deployment**: Defines the Firefly III application deployment, including its container specifications and update strategies.
- **Service**: Exposes the Firefly III application within the Kubernetes cluster and optionally to external clients.
- **PersistentVolumeClaim (PVC)**: Manages storage for Firefly III to ensure data persistence across pod restarts.
- **Secret**: Stores sensitive information such as passwords and API keys securely.
- **Ingress**: Configures external access to the Firefly III application, routing traffic from outside the Kubernetes cluster to the service.

## Setup Instructions

1. **Prepare Your Kubernetes Cluster**:
   Ensure you have a Kubernetes cluster up and running. This setup uses Talos as the operating system and ArgoCD for deployment management.

2. **Configure ArgoCD**:
   - Connect ArgoCD to your Git repository containing the Firefly III manifests.
   - Define the necessary projects and roles in ArgoCD to manage the deployment.

3. **Deploy Firefly III**:
   - Apply the Kubernetes manifests for Firefly III, including the ConfigMap, Deployment, Service, PVC, Secret, and Ingress.
   - Monitor the deployment using ArgoCD to ensure all resources are correctly applied and synchronized.

## Features

- **Automated Deployment**: Utilize ArgoCD to automate the deployment process and manage application lifecycle.
- **Persistent Storage**: Ensure data is stored persistently using Kubernetes PVC.
- **Secure Secrets**: Manage sensitive information securely using Kubernetes Secrets.
- **External Access**: Configure Ingress to provide external access to the Firefly III application.

## Use Cases

- **Personal Finance Management**: Use Firefly III to track and manage personal finances, including income, expenses, and financial goals.
- **Educational Purposes**: Learn about deploying applications on Kubernetes and managing them with ArgoCD.

## Contributing

Contributions are welcome! Please submit issues or pull requests to the GitHub repository. Ensure to follow best practices and test changes in a staging environment before applying them to production.
