# Kubernetes Platform Lab

![Kubernetes](https://img.shields.io/badge/Kubernetes-Platform-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)//img.shields.io/badge/Helm-Packages-0F1689?style=for-the-bo=helm&logoColor=white
![ArgoCD](https://img.shields.io/badge/ArgoCD-GitOps-EF7B4D?style=for-the-badge&logoColor=white
![Prometheus](https://img.shields.io/badge/Prometheus-Monitoring-E6522C?style=for-the-badge&logo=prometheuste
![Grafana](https://img.shields.io/badge/Grafana-Dashboards-F46800?style=forlogo=grafana&logoColor=white
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-CI/CD-2088FF?style=for-the-bctions&logoColor=white

Cloud-native Platform Engineering portfolio project demonstrating Kubernetes, Helm, GitOps, ArgoCD, Prometheus, Grafana, Kubernetes Secrets, GitHub Secrets, and Observability practices.

---

## Architecture

```text
GitHub Repository
        │
        ▼
     ArgoCD
        │
        ▼
 Kubernetes Cluster
        │
        ├── Namespace
        ├── Deployment
        ├── Service
        ├── Ingress
        ├── ConfigMap
        ├── Secret
        │
        ├── Prometheus
        │   ├── Alertmanager
        │   ├── Node Exporter
        │   └── Kube State Metrics
        │
        └── Grafana
```

---

## Features

✅ Kubernetes Deployments

✅ Services

✅ Ingress

✅ ConfigMaps

✅ Kubernetes Secrets

✅ GitHub Secrets Integration

✅ Helm Charts

✅ ArgoCD

✅ GitOps

✅ Prometheus

✅ Alertmanager

✅ Node Exporter

✅ Kube State Metrics

✅ Grafana

✅ Monitoring

✅ Observability

⏳ GitHub Actions Validation

---

## Screenshots

### ArgoCD GitOps

ArgoCD continuously synchronizes Kubernetes resources from Git.

![Ar/argocd-gitops.png

### Prometheus Metrics

Prometheus collecting Kubernetes and infrastructure metrics.

![Promrometheus-query.png

### Grafana Dashboard

Grafana visualizing Prometheus metrics and cluster health.

docs/grafana-dashboard.png

---

## Roadmap

### Phase 1 - Kubernetes Fundamentals

- [x] Namespace
- [x] Deployment
- [x] Service
- [x] Ingress

### Phase 2 - Configuration Management

- [x] ConfigMaps
- [x] Secret Templates
- [x] GitHub Secrets Integration

### Phase 3 - Package Management

- [x] Helm Charts

### Phase 4 - GitOps

- [x] ArgoCD
- [x] Automated Sync
- [x] Self Healing

### Phase 5 - Observability

- [x] Prometheus
- [x] Alertmanager
- [x] Node Exporter
- [x] Kube State Metrics
- [x] Grafana
- [x] Metrics Collection
- [x] Dashboard Visualization
- [x] Infrastructure Monitoring

### Phase 6 - CI/CD

- [ ] GitHub Actions
- [ ] yamllint
- [ ] kubeconform
- [ ] Kubernetes Manifest Validation

---

## Local Validation

Validate Kubernetes manifests:

```powershell
kubectl apply --dry-run=client --validate=false -f manifests/
```

Validate Helm chart:

```powershell
helm lint helm/nginx-chart

helm template nginx helm/nginx-chart
```

Validate ArgoCD application:

```powershell
kubectl get applications -n argocd

kubectl describe application nginx -n argocd
```

Verify observability stack:

```powershell
helm list -n platform-lab

kubectl get pods -n platform-lab
```

---

## Repository Structure

```text
kubernetes-platform-lab
│
├── .github/
│   └── workflows/
│
├── argocd/
│
├── docs/
│   ├── argocd-gitops.png
│   ├── grafana-dashboard.png
│   └── prometheus-query.png
│
├── helm/
│
├── manifests/
│
├── monitoring/
│
├── README.md
├── LICENSE
└── .gitignore
```

---

## Technologies

- Kubernetes
- Helm
- ArgoCD
- GitOps
- Prometheus
- Grafana
- GitHub Actions
- YAML
- Linux
- DevOps
- Platform Engineering
- Observability
- Monitoring
- Infrastructure Automation

---

## Status

🚧 Phase 6 In Progress