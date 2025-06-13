# 📦 Day 6: Kubernetes Basics

## 🧠 What is Kubernetes?

Kubernetes (K8s) is an **open-source container orchestration platform** that automates:

- **Deployment**
- **Scaling**
- **Load balancing**
- **Management of containerized applications**

It helps manage large numbers of containers in production environments.

---

## 🔧 Why is Kubernetes Needed?

| Problem with Docker Alone | Solution with Kubernetes |
|---------------------------|--------------------------|
| Difficult to scale        | Auto-scaling and load balancing |
| Manual deployment         | Automated deployments |
| No self-healing           | Kubernetes restarts failed containers |
| No service discovery      | Built-in DNS and service registry |

---

## 🚀 Key Concepts in Kubernetes:

| Term | Description |
|------|-------------|
| **Pod** | Smallest deployable unit, holds one or more containers |
| **Node** | A single machine (VM or physical) in a Kubernetes cluster |
| **Cluster** | Group of nodes managed by Kubernetes |
| **Deployment** | Controller that manages Pods |
| **Service** | Exposes your Pod to the network |
| **Kubelet** | Agent on each node |
| **kubectl** | Command-line tool to interact with the cluster |

---

## 📸 Screenshots of My Assignment

> Below are screenshots of my Kubernetes setup and commands:
![day 6 1](https://github.com/user-attachments/assets/f988b9c0-b74d-454d-8100-55ccf1e99e26)
![day 6 2](https://github.com/user-attachments/assets/93f17400-b0ff-4d2d-8c39-71928df92415)
![day6 3](https://github.com/user-attachments/assets/29b060fe-8e58-4e2d-8856-c7fc1e6831e6)
![day6 5](https://github.com/user-attachments/assets/cc4f872a-322b-4bf6-9a28-58abb83e740a)
![day 6 6](https://github.com/user-attachments/assets/4924d58f-ea58-4b6f-83d5-80a0c22bd422)


---

## 💡 What I Learned

- How to install and start Minikube (local Kubernetes cluster)
- Basic `kubectl` commands
- Creating a deployment and exposing it
- How Kubernetes manages containers more efficiently than Docker alone


---

## 🧰 Commands Used

```bash
minikube start
kubectl version
kubectl create deployment hello-node --image=k8s.gcr.io/echoserver:1.4
kubectl expose deployment hello-node --type=LoadBalancer --port=8080
kubectl get pods
kubectl get services
