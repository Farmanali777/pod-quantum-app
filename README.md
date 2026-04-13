# 🚀 Quantum Drug Discovery App on Kubernetes

This project demonstrates the deployment of a **Flask-based Quantum Drug Discovery application** using **Docker and Kubernetes**.

It showcases real-world DevOps practices including containerization, pod configuration, and port management.

---

## 🧱 Project Architecture

- Dockerized Flask Application
- Kubernetes Pod Deployment
- Port Forwarding for external access
- Custom container port configuration (8000)

---

## ⚙️ Technologies Used

- Python (Flask)
- Docker
- Kubernetes (kubectl, Pods)
- Linux (Ubuntu)
- Git & GitHub

---

## 🚀 How to Run

### 1️⃣ Clone the repository
```bash
git clone https://github.com/Farmanali777/pod-quantum-app.git
cd pod-quantum-app

# Apply the pod configuration
kubectl apply -f pod-quantum-app.yml

# View pod details
kubectl get pods

# Describe pod (for debugging)
kubectl describe pod quantum-app

# Check logs of the application
kubectl logs quantum-app

# Execute inside the container
kubectl exec -it quantum-app -- sh

# Port forward to access the app
kubectl port-forward --address 0.0.0.0 pod/quantum-app 8001:8000

<img width="1006" height="591" alt="image" src="https://github.com/user-attachments/assets/ae35f8c9-c624-4c93-9dec-4a26ad637589" />

<img width="1007" height="643" alt="image" src="https://github.com/user-attachments/assets/78f07aac-d452-4aa5-ad50-c48e8dab2221" />

<img width="1053" height="613" alt="image" src="https://github.com/user-attachments/assets/3da5049a-d20e-4789-81ff-54b937bd9b4c" />

# Delete pod (if needed)
kubectl delete pod quantum-app
