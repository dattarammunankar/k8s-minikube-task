# Kubernetes Namespace Exploration Task

This project demonstrates the setup of a local Kubernetes environment and the exploration of namespaces for resource isolation.

## 🛠 Tech Stack
* **Cloud Provider:** AWS EC2 (t2.medium)
* **OS:** Ubuntu 24.04 LTS
* **Container Runtime:** Docker
* **Orchestration:** Minikube & Kubectl

## 🚀 Execution Steps

### 1. Environment Setup
* Launched an EC2 t2.medium instance to satisfy Minikube's 2-vCPU requirement.
* Installed Docker as the primary driver for the Minikube cluster.

### 2. Namespace Creation
* Explored default namespaces (`default`, `kube-system`, etc.).
* Created a custom namespace named `dev-environment` for logical isolation.

### 3. Verification & Isolation
* Deployed an Nginx pod specifically into the `dev-environment` namespace.
* Verified that the pod is hidden from the `default` namespace but running successfully in the custom namespace.

## 📸 Proof of Work
Refer to the `/k8s-minikube-task`(screenshot) folder for:
1. Minikube cluster status and namespace creation.
2. Verified pod isolation within the custom namespace.
