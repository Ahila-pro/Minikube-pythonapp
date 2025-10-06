1. Prerequisites
    Minikube: minikube version

    kubectl: kubectl version --client

    Helm: helm version

    Docker (for building/pulling images)

    Ingress addon in Minikube: minikube addons enable ingress
2. minikube start --driver=docker --cpus=2 --memory=4096
3. minikube status  , minikube addons enable ingress
4. helm create minikube-pythonapp
5. Update values.yaml image /service /ingress
6. helm install minikube-pythonapp-v1 .
7. kubectl get pods  ,  kubectl get svc,  kubectl get ingress
8. minikube ip
9. Edit /etc/hosts:  <minikube-ip> minikubepythonapp.local
10.  check in browser http://minikubepythonapp.local 
