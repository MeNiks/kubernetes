# kubernetes
- kubectl apply -f any-file.yaml
  - service.yaml
  - deployment.yaml
  - config_map.yaml
  - namespace_creation.yaml,etc

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

# Kubectl

```
# kubectl apply -f namespace-integration.yaml
apiVersion: v1
kind: Namespace
metadata:
  name: integration
```



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
![image](https://github.com/user-attachments/assets/ddd5890e-7fa7-4135-bace-4e21b9c4fb72)

![image](https://github.com/user-attachments/assets/79414e3c-f360-4fa2-8e1a-7e693d4ce2d8)

![image](https://github.com/user-attachments/assets/bb731c27-c8d6-453d-ad65-1e541e987a76)

![image](https://github.com/user-attachments/assets/b44a1274-3a79-482a-b106-6bf5a26ee0ca)

![image](https://github.com/user-attachments/assets/6b5e116c-0594-4eb1-8005-00775d734191)

![image](https://github.com/user-attachments/assets/c302abfd-804d-42d5-a8bf-57d96d20c15d)


To install
- helm install --values=<my-values.yaml> <chart-name> --set version=1.0
- helm upgrade <chart-name>
  Ex - helm upgrate --install <name> <folder-name> --namespace integration -f <folder-name/values-config.yaml>
- helm rollback <chart-name>
