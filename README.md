
# 🚀 DevOps Project 2025

A hands-on **DevOps project** demonstrating:

- CI/CD automation using **GitHub Actions**
- Containerization with **Docker**
- Deployment to **Kubernetes**
- Infrastructure management using **Terraform** or **Ansible**
- Optional integration with **Prometheus & Grafana** for monitoring

---

## 🛠 Tech Stack

| Tool             | Purpose                     |
|------------------|-----------------------------|
| Git & GitHub     | Version control             |
| GitHub Actions   | CI/CD pipeline automation   |
| Docker           | Containerization            |
| Kubernetes       | Container orchestration     |
| Terraform / Ansible | Infrastructure as Code |
| Prometheus & Grafana | Monitoring & Observability |
| Trivy (optional) | Docker image vulnerability scanning |

---

## 📁 Project Structure

```bash
.
├── Dockerfile
├── main.tf / playbook.yml       # Terraform or Ansible config
├── deployment.yaml              # Kubernetes manifest
├── prometheus.yml / grafana/    # Monitoring configs
├── .github/workflows/
│   └── ci-cd.yml                # GitHub Actions pipeline
├── app.py / server.js / etc     # Application entry point
└── README.md
````

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/MohitMohanty2612/DevOps-Project-2025.git
cd DevOps-Project-2025
```

---

### 🐳 Run Locally with Docker

```bash
docker build -t devops-project .
docker run -d -p 8080:8080 devops-project
```

---

## ⚙️ CI/CD Pipeline – GitHub Actions

### 🔁 Triggered On:

* Every push to `main`
* Pull requests

### 🔧 What It Does:

* Lints & tests the code (if configured)
* Builds Docker image
* Scans image using **Trivy** (optional)
* Pushes Docker image to container registry
* Deploys to Kubernetes using `kubectl` or `helm`

---

### ✅ GitHub Secrets Required

Set these under **GitHub → Settings → Secrets and Variables → Actions**:

* `DOCKER_USERNAME`
* `DOCKER_PASSWORD`
* `KUBE_CONFIG_DATA` (base64-encoded kubeconfig)

---

## ☸️ Kubernetes Deployment (Optional)

Ensure you have `kubectl` configured and connected to your cluster.

```bash
kubectl apply -f deployment.yaml
```

Or with Helm:

```bash
helm install devops-project ./helm
```

---

## 📈 Monitoring (Optional)

* Configure Prometheus using `prometheus.yml`
* Setup Grafana dashboards from `/grafana/`
* Expose app metrics via `/metrics` endpoint

---

## 🤝 Contributing

Pull requests and suggestions are welcome!

> ⚠️ Please open an issue before making significant changes.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

###📸 Screenshots
<img width="1920" height="1020" alt="Screenshot 2025-07-26 013503" src="https://github.com/user-attachments/assets/254a1d64-2ee2-444c-9908-b2f8681f10db" />
<img width="1920" height="1020" alt="Screenshot 2025-07-26 014228" src="https://github.com/user-attachments/assets/a1468927-81a4-4239-9881-1e17884dfa68" />
<img width="1920" height="1020" alt="Screenshot 2025-07-26 014423" src="https://github.com/user-attachments/assets/6fd96a30-cfd0-4ddc-9a3f-b2a989eedee9" />
<img width="1920" height="1020" alt="Screenshot 2025-07-26 014503" src="https://github.com/user-attachments/assets/ee12b767-fb5e-43cb-9e63-8e9dfed58849" />
<img width="1920" height="1020" alt="Screenshot 2025-07-26 014643" src="https://github.com/user-attachments/assets/5b397a95-2cdd-41a2-a47a-219f68791112" />
<img width="1920" height="1020" alt="Screenshot 2025-07-26 014709" src="https://github.com/user-attachments/assets/66100cdc-3227-42b7-a083-6e8c092a0a84" />






