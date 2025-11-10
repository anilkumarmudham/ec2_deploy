# AWS EC2 Kubernetes Auto Deployment with Monitoring

## 🚀 Project Overview
This project demonstrates an **automated CI/CD pipeline** for deploying applications from **GitHub** to a **Kubernetes cluster** hosted on **AWS EC2 instances**.  
The setup includes **monitoring and logging** using **Prometheus, Grafana, and ELK Stack**, with an optional integration for **Datadog**.

---

## 🧱 Infrastructure Setup
The Kubernetes cluster consists of three EC2 instances:
| Instance Name | Role | Description |
|----------------|------|--------------|
| `k8s-instance-cp` | Control Plane (Master Node) | Manages the Kubernetes cluster, API server, scheduler, and controller manager. |
| `k8s-instance-1` | Worker Node | Runs the deployed application workloads (Pods). |
| `k8s-instance-2` | Worker Node | Additional worker node for scaling and redundancy. |

---

## ⚙️ Continuous Deployment Workflow
1. **Code Push** → Developer pushes code to the GitHub repository.
2. **GitHub Action / Webhook Trigger** → Automatically triggers deployment workflow.
3. **Kubernetes Deployment** → Updated application is deployed across EC2 worker nodes.
4. **Monitoring & Logging** → Metrics and logs are collected and visualized.

---

## 🧩 Tools & Technologies
| Category | Tools Used | Purpose |
|-----------|-------------|----------|
| **Version Control** | Git & GitHub | Source code management |
| **Infrastructure** | AWS EC2 | Hosts the Kubernetes cluster |
| **Container Orchestration** | Kubernetes | Application deployment & scaling |
| **Monitoring** | Prometheus + Grafana | Metrics collection & visualization |
| **Logging** | ELK Stack (Elasticsearch, Logstash, Kibana) | Centralized log management |
| **Optional Monitoring** | Datadog | Cloud-based performance monitoring |

---

## 🔄 Future Enhancements
- Integrate **GitHub Actions** or **ArgoCD** for CI/CD automation  
- Add **AlertManager** for Prometheus alerts  
- Implement **Datadog agent** for unified observability  
- Add **Terraform** for Infrastructure as Code (IaC)

---

## 🧠 Learning Objectives
- Automate deployment pipelines from GitHub to Kubernetes.
- Configure metrics & log monitoring on EC2 instances.
- Understand end-to-end DevOps workflow (Code → Deploy → Observe).

---

## 👨‍💻 Author
**Anil Kumar Mudham**  
DevOps Enthusiast | AWS | Kubernetes | Monitoring | CI/CD Automation
