# API Python no Kubernetes

## Atividade

Subir a API Python em um cluster Kubernetes com:
- Deployment (2 pods)
- Service
- Ingress

## Repositorio clonado

https://github.com/profdiegocbcastro/gerencia-de-config.git

## Comandos

```bash
docker build -t api-python:latest .
minikube image load api-python:latest

kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml
kubectl apply -f k8s/ingress.yaml

kubectl get pods
kubectl get svc
kubectl get ingress
```
