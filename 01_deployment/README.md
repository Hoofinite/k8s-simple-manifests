# Nginx Server Deployment in Kubernetes

Welcome to the repository containing the YAML manifest for deploying the Nginx server version 1.9 on a Minikube cluster. This deployment is configured to run 5 replicas of the server.

## Repository Structure

The repository includes the file `nginx-deployment.yaml`, which contains all necessary configurations:

- **Deployment** - Configures the deployment of the Nginx server using the image in version 1.9.
- **Replicas** - Configures the amount of replicas of the Nginx server to 5.
- **Update Strategy** - Update strategy parameters are designed to ensure that no more than 2 Pods are unavailable during the update process.

## Usage

Assuming you have Minikube installed and configured appropriately, to apply following Nginx deployment in your cluster, use the following command:

```bash
kubectl apply -f nginx-deployment.yaml
