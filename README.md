# rnd-kubernetes

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

minikube ip

# Other resources
Go Highly Available (H/A) etcd
Kubernetes LoadBalancer Services
CoreOS rkt, Docker, GKE
