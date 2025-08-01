# Kubernetes Learning Lab: From Pods to EKS

This repository documents my end-to-end journey learning Kubernetes — starting from core concepts like Pods and Deployments, to advanced topics like Helm, Ingress Controllers, Operators, and deploying a complete application on AWS EKS. Each folder demonstrates a key concept or milestone in mastering Kubernetes.

---

## 🧭 Project Overview

- **Goal**: Understand and implement core to advanced Kubernetes features in a hands-on, structured way.
- **Approach**: Start with local deployments using `kubectl` and `minikube`, then progress to Helm and AWS EKS for real-world production deployment experience.

---

## 🗂️ Folder Structure & Modules

| Folder | Topic | Description |
|--------|-------|-------------|
| `01-pods-containers` | Pods & Containers | Created basic Kubernetes Pods using YAML files to run simple containerized applications. |
| `02-service-discovery` | Services | Implemented ClusterIP, NodePort, and LoadBalancer services for service discovery and communication. |
| `03-namespaces` | Namespaces | Segmented cluster resources using Namespaces to simulate multi-tenant architecture. |
| `04-deployments-pod-replicas` | Deployments | Created Deployments and ReplicaSets for self-healing and scaling of Pods. |
| `05-liveness-readiness-probes` | Health Checks | Used liveness and readiness probes to monitor and manage container health. |
| `06-stateful-pv` | Persistent Storage | Used PersistentVolumes and PersistentVolumeClaims for data persistence. |
| `07-configMap-secrets` | Config & Secrets | Managed application configuration securely using ConfigMaps and Secrets. |
| `08-hori-pod-autosc` | Horizontal Pod Autoscaler | Enabled autoscaling based on CPU utilization to ensure optimal performance. |
| `09-ingress-controller` | Ingress Routing | Set up NGINX Ingress Controller for routing external traffic to services with path-based routing and TLS. |
| `10-helm-charts` | Helm Chart Creation | Packaged Kubernetes applications using Helm templates for consistent and repeatable deployments. |
| `11-helm-pkg-man` | Helm & AWS EKS | Deployed Helm-managed applications to a production-grade AWS EKS cluster. |
| `12-k8s-operator` | Kubernetes Operator | Used a Kubernetes Operator to automate MongoDB deployment and configuration. |

---

## 🚀 Deployment Highlights

- **Tooling**: `kubectl`, `minikube`, `Helm`, `AWS CLI`, `eksctl`
- **Cloud Platform**: AWS Elastic Kubernetes Service (EKS)
- **CI/CD Potential**: Ready for integration with GitOps tools like ArgoCD or FluxCD

---

## 📌 Technologies Used

- Kubernetes (v1.25+)
- Helm 3
- AWS EKS
- Docker
- NGINX Ingress Controller
- MongoDB Operator
- ConfigMaps, Secrets, PVs, HPA, etc.

---

## 🧪 How to Run

> Pre-requisites:
> - Docker
> - `kubectl`
> - `minikube` or an existing K8s cluster
> - `helm`
> - AWS CLI configured (for EKS modules)

### Example:
```bash
kubectl apply -f 01-pods-containers/
kubectl get pods

kubectl apply -f 04-deployments-pod-replicas/
kubectl scale deployment <deployment-name> --replicas=3




