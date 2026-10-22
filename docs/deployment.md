# Deployment - PlayBook (24ESKCS082)

- Live URL: https://skit-devops-2026.github.io/devops-24ESKCS082/
- Source: this repository (skit-devops-2026/devops-24ESKCS082), deployed with
  GitHub Pages through the "Deploy to GitHub Pages" workflow
  (.github/workflows/pages.yml) on every push to main.
- Container image: ghcr.io/skit-devops-2026/devops-24eskcs082:latest
  (built and pushed by the CI workflow on every push to main).

## Local deployment with Docker

```bash
docker compose up --build
# site:        http://localhost:8080
# health:      http://localhost:8080/health
# Prometheus:  http://localhost:9090
# Grafana:     http://localhost:3000
```

## Kubernetes

```bash
kubectl apply -f k8s/
```
