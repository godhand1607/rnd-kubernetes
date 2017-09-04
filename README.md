# rnd-kubernetes

## Local Environment Setup
1. minikube
1. kubectl

## Minikube
Starting the minikube vm:
```
minikube start
```

Checking the minikube vm status:
```
minikube status
```

Stopping the minikube vm:
```
minikube stop
```

Viewing the ip address of the minikube vm:
```
minikube ip
```

Viewing the dashboard:
```
minikube dashboard
```

View a service/app:
```
minikube service <servicename>
```

## kubectl
    CLI to access any kubernetes cluster

View config:
```
kubectl config view
```

Access the minikube(or any context) api's:
```
kubectl proxy
```

kubectl config current-context

kubectl get pods|nodes|rc|svc|deploy|rs

kubectl describe pods|nodes|rc|svc|deploy|rs

kubectl create deployment

# Create
kubectl create -f "filepathhere"

# Update
kubectl apply -f "filepathhere" --record
kubectl rollout status deployment "deploymentnamehere"
kubectl rollout history deployment "deploymentnamehere"

# Rollback
kubetctl rollout undo deployment hello-deploy --to-revision=1

Always use --record

rc = replicationController
svc = service
rs = replicaSet


### Monitoring
- Heapster
- Prometheus

### Logging
- Elasticsearch
- fluentd

# Other resources
Go Highly Available (H/A) etcd
Kubernetes LoadBalancer Services
CoreOS rkt, Docker, GKE
