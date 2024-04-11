# App hello world Spring Boot, PostgreSQL avec Docker, kubernetes et minikube

## Etapes kubernetes et minikube
```
minikube start
minikube dashboard
kubectl apply -f kubernetes-namespace.yaml
kubectl apply -f database/database-service.yaml
kubectl apply -f database/database-deployment.yaml
kubectl apply -f database/database-secrets.yaml
kubectl apply -f database/database-volume.yaml
kubectl apply -f database/database-config-map.yaml
minikube image build -t helloworld:0.0.1 .