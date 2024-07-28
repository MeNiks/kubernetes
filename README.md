# kubernetes
kubernetes



# minikube
 - https://minikube.sigs.k8s.io/docs/start/

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



M1
- curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-darwin-arm64
- sudo install minikube-darwin-arm64 /usr/local/bin/minikube
- minikube start --driver=docker --alsologtostderr
- docker ps | grep minikube
- minikube delete --all --purge
