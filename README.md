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


M1
- curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-darwin-arm64
- sudo install minikube-darwin-arm64 /usr/local/bin/minikube
- minikube start --driver=docker --alsologtostderr
- docker ps | grep minikube
- minikube delete --all --purge


# Helm
Is used to managed flavours ex- integration/staging/prod
Has folders
- values.yaml
- values-integration.yaml
- values-prod.yaml
Also used for templating
![image](https://github.com/user-attachments/assets/bb75aac9-a1b8-49b2-a566-1a19dff1ecf9)


To install
- 
