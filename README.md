<div align="center">

# 🚀 Resume AI Update

### AI-Powered Resume Tailoring Platform

**End-to-End DevOps Deployment using Docker, Docker Compose, Kubernetes, Ingress & HTTPS**

<br/>

![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github)
![Docker](https://img.shields.io/badge/Docker-Containerized-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestrated-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python&logoColor=white)
![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-Web_Server-009639?style=for-the-badge&logo=nginx&logoColor=white)

<br/>

![Status](https://img.shields.io/badge/Project_Status-Completed-success?style=flat-square)
![Deployment](https://img.shields.io/badge/Deployment-Kubernetes-blue?style=flat-square)
![HTTPS](https://img.shields.io/badge/HTTPS-Let's_Encrypt-success?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)

<br/><br/>

### 🌐 Production

**Frontend:**  
`https://venugopalareddy.in`

**Backend API:**  
`https://api.venugopalareddy.in`

</div>

---

# 📌 Project Overview

**Resume AI Update** is a full-stack AI-powered resume tailoring application designed to help users create, manage, analyze, and improve resumes.

The project was converted into a complete **DevOps deployment pipeline**, covering the entire journey from source code to production-style Kubernetes deployment.

The implementation demonstrates:

- Source Code Management
- Application Development
- Docker Containerization
- Multi-Container Orchestration
- Container Registry
- Kubernetes Deployment
- Service Discovery
- Ingress Routing
- DNS Configuration
- HTTPS/TLS
- ConfigMap
- Kubernetes Secrets
- Health Checks
- Scaling
- Self-Healing
- End-to-End Testing

---

# 🏗️ Architecture

```text
                         ┌──────────────────────┐
                         │       GitHub         │
                         │    Source Code       │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │    Docker Build      │
                         └──────────┬───────────┘
                                    │
                    ┌───────────────┴───────────────┐
                    ▼                               ▼
          ┌──────────────────┐            ┌──────────────────┐
          │ Backend Image    │            │ Frontend Image   │
          │ FastAPI/Python   │            │ React + Nginx    │
          └────────┬─────────┘            └────────┬─────────┘
                   │                               │
                   └──────────────┬────────────────┘
                                  ▼
                         ┌──────────────────┐
                         │    Docker Hub    │
                         │ Container Registry│
                         └────────┬─────────┘
                                  │
                                  ▼
                    ┌──────────────────────────┐
                    │    Kubernetes Cluster    │
                    │         kubeadm          │
                    └────────────┬─────────────┘
                                 │
                 ┌───────────────┴───────────────┐
                 ▼                               ▼
       ┌──────────────────┐             ┌──────────────────┐
       │ Backend Deployment│             │Frontend Deployment│
       │    2 Replicas    │             │    2 Replicas    │
       └────────┬─────────┘             └────────┬─────────┘
                │                                │
                ▼                                ▼
       ┌──────────────────┐             ┌──────────────────┐
       │ Backend Service  │             │Frontend Service  │
       │    ClusterIP     │             │    ClusterIP     │
       │      :8000       │             │       :80        │
       └────────┬─────────┘             └────────┬─────────┘
                │                                │
                └───────────────┬────────────────┘
                                ▼
                       ┌──────────────────┐
                       │  Ingress-NGINX   │
                       └────────┬─────────┘
                                │
                  ┌─────────────┴─────────────┐
                  ▼                           ▼
       ┌────────────────────┐      ┌────────────────────────┐
       │venugopalareddy.in  │      │api.venugopalareddy.in  │
       │     Frontend       │      │       Backend API      │
       └────────────────────┘      └────────────────────────┘
                  │                           │
                  └─────────────┬─────────────┘
                                ▼
                         ┌──────────────┐
                         │ HTTPS / TLS  │
                         │ Let's Encrypt│
                         └──────────────┘
````

---

# 🔄 DevOps Workflow

```text
Source Code
     │
     ▼
   GitHub
     │
     ▼
Docker Build
     │
     ├──────────────┐
     ▼              ▼
 Backend         Frontend
 Docker Image    Docker Image
     │              │
     └───────┬──────┘
             ▼
         Docker Hub
             │
             ▼
      Kubernetes Cluster
             │
       ┌─────┴─────┐
       ▼           ▼
    Backend      Frontend
   Deployment   Deployment
       │           │
       ▼           ▼
    Service      Service
       │           │
       └─────┬─────┘
             ▼
        Ingress-NGINX
             │
             ▼
        HTTPS / DNS
             │
             ▼
          End User
```

---

# 🧰 Tech Stack

## Frontend

| Technology | Purpose               |
| ---------- | --------------------- |
| React.js   | UI                    |
| Vite       | Frontend build tool   |
| JavaScript | Application logic     |
| Nginx      | Production web server |

## Backend

| Technology | Purpose          |
| ---------- | ---------------- |
| Python     | Backend language |
| FastAPI    | REST API         |
| Uvicorn    | ASGI server      |
| SQLite     | Database         |

## AI

| Technology       | Purpose              |
| ---------------- | -------------------- |
| Anthropic Claude | AI Resume Processing |
| OpenAI           | AI Resume Processing |
| Ollama           | Local AI Support     |

## DevOps

| Technology     | Purpose                       |
| -------------- | ----------------------------- |
| Git            | Version Control               |
| GitHub         | Source Code Repository        |
| Docker         | Containerization              |
| Docker Compose | Multi-container orchestration |
| Docker Hub     | Container Registry            |
| Kubernetes     | Container orchestration       |
| kubeadm        | Kubernetes cluster setup      |
| Nginx Ingress  | External routing              |
| cert-manager   | TLS automation                |
| Let's Encrypt  | SSL certificates              |

## Cloud

| Technology          | Purpose                   |
| ------------------- | ------------------------- |
| AWS EC2             | Kubernetes infrastructure |
| AWS Security Groups | Network security          |
| DNS                 | Domain routing            |

---

# 📂 Project Structure

```text
resume-ai-update/
│
├── backend/
│   ├── app/
│   │   ├── main.py
│   │   ├── ai_service.py
│   │   ├── ats_service.py
│   │   ├── auth.py
│   │   ├── database.py
│   │   ├── export_service.py
│   │   ├── models.py
│   │   ├── rate_limits.py
│   │   ├── schemas.py
│   │   │
│   │   └── routers/
│   │       ├── admin.py
│   │       ├── auth_router.py
│   │       ├── dashboard.py
│   │       ├── export.py
│   │       ├── history.py
│   │       ├── resumes.py
│   │       ├── settings.py
│   │       └── versions.py
│   │
│   ├── requirements.txt
│   ├── Dockerfile
│   ├── .dockerignore
│   └── .env.example
│
├── frontend/
│   ├── src/
│   │   ├── App.jsx
│   │   ├── api.js
│   │   ├── main.jsx
│   │   ├── resumeFormat.jsx
│   │   ├── index.css
│   │   │
│   │   └── components/
│   │       ├── AdminDashboard.jsx
│   │       ├── Dashboard.jsx
│   │       ├── History.jsx
│   │       ├── Login.jsx
│   │       ├── ResumeApp.jsx
│   │       ├── ResumePreview.jsx
│   │       ├── SectionOrderList.jsx
│   │       ├── Settings.jsx
│   │       ├── Sidebar.jsx
│   │       └── TemplateGrid.jsx
│   │
│   ├── package.json
│   ├── package-lock.json
│   ├── vite.config.js
│   ├── index.html
│   ├── Dockerfile
│   └── .dockerignore
│
├── k8s/
│   ├── backend-configmap.yaml
│   ├── backend-secret.example.yaml
│   ├── backend-deployment.yaml
│   ├── backend-service.yaml
│   ├── frontend-deployment.yaml
│   ├── frontend-service.yaml
│   ├── ingress.yaml
│   └── clusterissuer.yaml
│
├── docker-compose.yml
├── .gitignore
└── README.md
```

---

# 🐳 Docker

## Backend Image

```dockerfile
FROM python:3.12-slim

WORKDIR /app

ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY app ./app

EXPOSE 8000

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]
```

Build:

```bash
cd backend

docker build \
  -t resume-ai-backend:1.0 .
```

---

## Frontend Image

The frontend uses a **multi-stage Docker build**.

```dockerfile
FROM node:20-alpine AS builder

WORKDIR /app

COPY package*.json .

RUN npm ci

COPY . .

ARG VITE_API_BASE_URL
ENV VITE_API_BASE_URL=$VITE_API_BASE_URL

RUN npm run build


FROM nginx:alpine

COPY --from=builder /app/dist /usr/share/nginx/html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
```

Build:

```bash
cd frontend

docker build \
  --build-arg VITE_API_BASE_URL=https://api.venugopalareddy.in \
  -t resume-ai-frontend:1.2 .
```

---

# 🐋 Docker Compose

Docker Compose is used to run the frontend and backend together during multi-container testing.

```yaml
services:

  backend:
    build:
      context: ./backend
      dockerfile: Dockerfile

    container_name: resume-ai-backend

    ports:
      - "8000:8000"

    restart: unless-stopped

    volumes:
      - backend-data:/app


  frontend:
    build:
      context: ./frontend
      dockerfile: Dockerfile

      args:
        VITE_API_BASE_URL: http://localhost:8000

    container_name: resume-ai-frontend

    ports:
      - "5173:80"

    restart: unless-stopped

    depends_on:
      - backend


volumes:
  backend-data:
```

Start:

```bash
docker compose up -d
```

Check:

```bash
docker compose ps
```

Logs:

```bash
docker compose logs -f
```

Stop:

```bash
docker compose down
```

---

# 📦 Docker Hub

Images:

```text
<YOUR_DOCKERHUB_USERNAME>/resume-ai-backend:1.0
<YOUR_DOCKERHUB_USERNAME>/resume-ai-frontend:1.2
```

Login:

```bash
docker login
```

Tag:

```bash
docker tag resume-ai-backend:1.0 \
<YOUR_DOCKERHUB_USERNAME>/resume-ai-backend:1.0
```

```bash
docker tag resume-ai-frontend:1.2 \
<YOUR_DOCKERHUB_USERNAME>/resume-ai-frontend:1.2
```

Push:

```bash
docker push \
<YOUR_DOCKERHUB_USERNAME>/resume-ai-backend:1.0
```

```bash
docker push \
<YOUR_DOCKERHUB_USERNAME>/resume-ai-frontend:1.2
```

---

# ☸️ Kubernetes

## Backend Deployment

```yaml
apiVersion: apps/v1
kind: Deployment

metadata:
  name: resume-ai-backend

spec:
  replicas: 2

  selector:
    matchLabels:
      app: resume-ai-backend

  template:
    metadata:
      labels:
        app: resume-ai-backend

    spec:
      containers:

        - name: backend

          image: <YOUR_DOCKERHUB_USERNAME>/resume-ai-backend:1.0

          ports:
            - containerPort: 8000

          envFrom:

            - configMapRef:
                name: resume-ai-backend-config

            - secretRef:
                name: resume-ai-backend-secret

          resources:

            requests:
              cpu: "100m"
              memory: "128Mi"

            limits:
              cpu: "500m"
              memory: "512Mi"

          readinessProbe:
            httpGet:
              path: /
              port: 8000

          livenessProbe:
            httpGet:
              path: /
              port: 8000
```

---

# 🌐 Kubernetes Services

## Backend

```yaml
apiVersion: v1
kind: Service

metadata:
  name: resume-ai-backend

spec:
  selector:
    app: resume-ai-backend

  ports:
    - port: 8000
      targetPort: 8000

  type: ClusterIP
```

## Frontend

```yaml
apiVersion: v1
kind: Service

metadata:
  name: resume-ai-frontend

spec:
  selector:
    app: resume-ai-frontend

  ports:
    - port: 80
      targetPort: 80

  type: ClusterIP
```

---

# 🌍 Ingress

The application uses two hostnames.

```yaml
apiVersion: networking.k8s.io/v1

kind: Ingress

metadata:
  name: resume-ai-ingress

  annotations:
    cert-manager.io/cluster-issuer: letsencrypt-prod
    nginx.ingress.kubernetes.io/ssl-redirect: "true"

spec:

  ingressClassName: nginx

  tls:

    - hosts:
        - venugopalareddy.in
        - api.venugopalareddy.in

      secretName: resume-ai-tls

  rules:

    - host: venugopalareddy.in

      http:
        paths:

          - path: /

            pathType: Prefix

            backend:

              service:
                name: resume-ai-frontend
                port:
                  number: 80


    - host: api.venugopalareddy.in

      http:
        paths:

          - path: /

            pathType: Prefix

            backend:

              service:
                name: resume-ai-backend
                port:
                  number: 8000
```

---

# 🔐 ConfigMap

Non-sensitive configuration is stored in a Kubernetes ConfigMap.

```yaml
apiVersion: v1
kind: ConfigMap

metadata:
  name: resume-ai-backend-config

data:

  CORS_ORIGINS: "https://venugopalareddy.in"

  DATABASE_URL: "sqlite:///./resume_tailor.db"

  OPENAI_MODEL: "gpt-4o-mini"

  ANTHROPIC_MODEL: "claude-sonnet-4-5"

  OLLAMA_BASE_URL: "http://127.0.0.1:11434"

  OLLAMA_MODEL: "llama3.2:1b"
```

Apply:

```bash
kubectl apply -f k8s/backend-configmap.yaml
```

---

# 🔑 Kubernetes Secrets

Sensitive credentials are stored using Kubernetes Secrets.

```yaml
apiVersion: v1
kind: Secret

metadata:
  name: resume-ai-backend-secret

type: Opaque

stringData:

  JWT_SECRET_KEY: "CHANGE_ME"

  OPENAI_API_KEY: ""

  ANTHROPIC_API_KEY: ""
```

### Security

The real secret file must **never be committed to GitHub**.

Add:

```gitignore
k8s/backend-secret.yaml
```

Commit only:

```text
backend-secret.example.yaml
```

---

# 🔒 HTTPS / TLS

TLS is automated using:

* cert-manager
* Let's Encrypt
* Ingress-NGINX

Certificate:

```text
resume-ai-tls
```

Domains:

```text
venugopalareddy.in
api.venugopalareddy.in
```

Check:

```bash
kubectl get certificate
```

Expected:

```text
NAME            READY
resume-ai-tls   True
```

---

# 🚀 Kubernetes Deployment

Apply all manifests:

```bash
kubectl apply -f k8s/backend-configmap.yaml

kubectl apply -f k8s/backend-secret.yaml

kubectl apply -f k8s/backend-deployment.yaml

kubectl apply -f k8s/backend-service.yaml

kubectl apply -f k8s/frontend-deployment.yaml

kubectl apply -f k8s/frontend-service.yaml

kubectl apply -f k8s/ingress.yaml

kubectl apply -f k8s/clusterissuer.yaml
```

---

# 🔍 Kubernetes Verification

Check nodes:

```bash
kubectl get nodes
```

Check pods:

```bash
kubectl get pods -o wide
```

Check deployments:

```bash
kubectl get deployments
```

Check services:

```bash
kubectl get svc
```

Check ingress:

```bash
kubectl get ingress
```

Check certificates:

```bash
kubectl get certificate
```

---

# ❤️ Health Checks

Backend health:

```bash
curl https://api.venugopalareddy.in/
```

Expected:

```json
{
  "status": "ok",
  "service": "resume-tailor-api"
}
```

Swagger:

```text
https://api.venugopalareddy.in/docs
```

Frontend:

```text
https://venugopalareddy.in
```

---

# 📈 Kubernetes Scaling

Scale backend:

```bash
kubectl scale deployment resume-ai-backend --replicas=3
```

Verify:

```bash
kubectl get pods -l app=resume-ai-backend
```

Scale back:

```bash
kubectl scale deployment resume-ai-backend --replicas=2
```

---

# ♻️ Self-Healing Test

Delete a backend pod:

```bash
kubectl delete pod <POD_NAME>
```

Watch:

```bash
kubectl get pods -l app=resume-ai-backend -w
```

Kubernetes automatically creates a replacement pod.

This demonstrates Kubernetes **self-healing**.

---

# 🧪 Testing

| Test                  | Status |
| --------------------- | :----: |
| Local Backend         |    ✅   |
| Local Frontend        |    ✅   |
| Docker Backend        |    ✅   |
| Docker Frontend       |    ✅   |
| Docker Compose        |    ✅   |
| Docker Hub Push       |    ✅   |
| Docker Hub Pull       |    ✅   |
| Kubernetes Deployment |    ✅   |
| Kubernetes Services   |    ✅   |
| Ingress               |    ✅   |
| DNS                   |    ✅   |
| HTTPS/TLS             |    ✅   |
| ConfigMap             |    ✅   |
| Kubernetes Secret     |    ✅   |
| Backend API           |    ✅   |
| Swagger UI            |    ✅   |
| Frontend → Backend    |    ✅   |
| Scaling               |    ✅   |
| Self-Healing          |    ✅   |

---

# 📸 Screenshots

Recommended project evidence:

```text
docs/
├── 01-local-application.png
├── 02-docker-images.png
├── 03-docker-compose.png
├── 04-docker-hub.png
├── 05-kubernetes-nodes.png
├── 06-kubernetes-pods.png
├── 07-kubernetes-services.png
├── 08-ingress.png
├── 09-configmap.png
├── 10-secrets.png
├── 11-tls-certificate.png
├── 12-frontend.png
├── 13-backend-api.png
├── 14-swagger.png
├── 15-scaling.png
└── 16-self-healing.png
```

> Do not include screenshots containing passwords, API keys, JWT secrets, private keys, or other sensitive information.

---

# 🛠️ Troubleshooting

## ImagePullBackOff

```bash
kubectl describe pod <POD_NAME>
```

Check:

* Docker Hub username
* Image name
* Image tag
* Repository visibility

---

## CrashLoopBackOff

```bash
kubectl logs <POD_NAME>
```

Then:

```bash
kubectl describe pod <POD_NAME>
```

---

## Service Not Working

```bash
kubectl get endpoints
```

Check pod labels:

```bash
kubectl get pods --show-labels
```

---

## Ingress Problems

```bash
kubectl get ingress
```

```bash
kubectl describe ingress resume-ai-ingress
```

Check controller:

```bash
kubectl get pods -n ingress-nginx
```

---

## TLS Certificate Problems

```bash
kubectl get certificate
```

```bash
kubectl get challenges
```

```bash
kubectl describe certificate resume-ai-tls
```

---

# 🔐 Security Practices

This project implements:

* HTTPS/TLS
* Let's Encrypt certificates
* Kubernetes Secrets
* ConfigMaps
* CORS configuration
* Resource limits
* Readiness probes
* Liveness probes
* Private ClusterIP backend
* Docker `.dockerignore`
* Git `.gitignore`
* No API keys in source code
* No `.env` files in Git
* No Kubernetes secret manifests containing real credentials in Git

---

# 📊 DevOps Skills Demonstrated

```text
                    DEVOPS SKILLS
                         │
       ┌─────────────────┼─────────────────┐
       │                 │                 │
       ▼                 ▼                 ▼
   Source Control    Containerization   Kubernetes
       │                 │                 │
     Git              Docker          Deployments
     GitHub           Compose          Services
       │              Docker Hub        Ingress
       │                                ConfigMap
       │                                Secrets
       │                                Scaling
       │                                Self-Healing
       │
       └─────────────────┬─────────────────┘
                         │
                         ▼
                  Cloud Deployment
                         │
                      AWS EC2
                         │
                         ▼
                    HTTPS / TLS
```

---

# 🚀 Future Enhancements

The project can be further improved with:

* GitHub Actions CI/CD
* Automated Docker builds
* Automated Kubernetes deployment
* Prometheus
* Grafana
* Kubernetes HPA
* Centralized logging
* AWS Load Balancer
* AWS Secrets Manager
* External Secrets Operator
* PostgreSQL / Amazon RDS
* Terraform infrastructure
* Ansible automation
* SonarQube
* Snyk security scanning
* Argo CD
* GitOps workflow

---

# 🎯 Project Outcomes

By completing this project, the following practical DevOps concepts were implemented:

### Source Control

* Git
* GitHub
* Branching
* `.gitignore`

### Containerization

* Dockerfiles
* Multi-stage builds
* Docker images
* Docker containers
* Docker networks
* Docker volumes

### Orchestration

* Docker Compose
* Kubernetes
* Deployments
* Services
* Replicas
* Scaling
* Self-healing

### Networking

* ClusterIP
* NodePort
* Ingress
* DNS
* Domain routing

### Security

* HTTPS
* TLS
* Let's Encrypt
* cert-manager
* ConfigMaps
* Kubernetes Secrets
* CORS

### Cloud

* AWS EC2
* Security Groups
* DNS

---

# 👨‍💻 Author

<div align="center">

## Venu Gopala Reddy Eppala

### Cloud & DevOps Engineer

AWS • Docker • Kubernetes • Terraform • CI/CD • Linux • Python

<br/>

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/<YOUR_GITHUB_USERNAME>)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge\&logo=linkedin\&logoColor=white)](https://www.linkedin.com/in/<YOUR_LINKEDIN_USERNAME>/)

[![Portfolio](https://img.shields.io/badge/Portfolio-venugopalareddy.in-000000?style=for-the-badge\&logo=googlechrome\&logoColor=white)](https://venugopalareddy.in)

</div>

---

# ⭐ Project Summary

> **Resume AI Update demonstrates a complete end-to-end DevOps implementation, transforming a full-stack AI application into a containerized, Kubernetes-orchestrated, HTTPS-secured production-style application.**

```text
GitHub
  ↓
Docker
  ↓
Docker Compose
  ↓
Docker Hub
  ↓
Kubernetes
  ↓
Ingress
  ↓
DNS
  ↓
Let's Encrypt
  ↓
HTTPS
  ↓
Production Application
```

---

<div align="center">

### 🚀 Built with DevOps • Cloud • Containers • Kubernetes

**Resume AI Update**

⭐ Star the repository if you found this project useful!

</div>
```

### Recommended repository presentation

For an even more polished GitHub repository, put these at the top:

```text
README.md
│
├── 🚀 Project banner
├── 📊 Badges
├── 🌐 Live URLs
├── 📌 Overview
├── 🏗️ Architecture
├── 🧰 Tech Stack
├── 📂 Project Structure
├── 🐳 Docker
├── 🐋 Docker Compose
├── 📦 Docker Hub
├── ☸️ Kubernetes
├── 🌍 Ingress
├── 🔐 ConfigMap & Secrets
├── 🔒 HTTPS/TLS
├── 🧪 Testing
├── 📸 Screenshots
├── 🛠️ Troubleshooting
├── 📈 Scaling & Self-Healing
├── 🚀 Future Enhancements
└── 👨‍💻 Author
```
