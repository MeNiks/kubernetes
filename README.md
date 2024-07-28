# kubernetes
kubernetes



# minikube
 - https://minikube.sigs.k8s.io/docs/start/

# Commands
- brew install kubectl
- brew install hyperkit
- brew install minikube
- brew list
  - You should see kubernetes-cli
- minikube version
- minikube start
  - This will pick default driver
- or
- minikube start hyperkit
- minikube status
- minikube dashboard
- minikube status
- kubectl cluster-info
- kubectl get nodes
- minikube delete
- eval $(minikube docker-env) # to build docker image locally and deploy on minikube cluster


M1
- curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-darwin-arm64
- sudo install minikube-darwin-arm64 /usr/local/bin/minikube
- minikube start --driver=docker --alsologtostderr
- docker ps | grep minikube
- minikube delete --all --purge
