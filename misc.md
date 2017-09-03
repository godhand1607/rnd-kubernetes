---
# Minikube Pipeline
minikube start
kubectl get pod|deployment|services

# Get exposed container ip & port of a deployment/pod
minikube service <deployment> --url

# Check the status of a pod
kubectl describe pod <pod-name>

# Login to Node Cluster
minikube ssh

# SSH to a Pod
kubectl exec -it <pod-name> — /bin/bash

# Helm + Tiller Server
helm init

# Kubeadm - Pipeline kubeadm init
sudo cp /etc/kubernetes/admin.conf $HOME/ && sudo chown $(id -u):$(id -g) $HOME/admin.conf && export KUBECONFIG=$HOME/admin.conf
kubeadm join —token <11111> --skip-preflight-checks
kubectl taint nodes --all node-role.kubernetes.io/master- kubectl apply -f https://git.io/weave-kube-1.6 

kubectl Config
kubectl config view 

# Set Namepace In KubeAdm Config
kubectl config set-context $(kubectl config current-context) --namespace=mckinsey

# Kubectl Get Service Endpoint
kubetl get ep <service-name>

# KubeAdm TearDown
kubectl drain ip-172-31-70-227 --delete-local-data --force --ignore-daemonsets
kubectl delete node ip-172-31-70-227
kubeadm reset

# Delete All Services|Deployments|Pods in A Namespace 

kubectl delete --all services --namespace=mckinsey
