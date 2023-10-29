Comandos para usar caso perca o ambiente e tenha que criar de novo

Iniciar ambiente kubernetes
kind create cluster --config=k8s/kind.yaml --name=fullcycle
kubectl cluster-info --context kind-fullcycle
kind get clusters
kubectl config get-clusters

docker ps 
kubectl apply -f k8s/deployment.yaml
kubectl get pods
kubectl logs goserver-5cbbd7db8d-pr7cp
kubectl apply -f k8s/secret.yaml
kubectl apply -f k8s/service.yaml
kubectl get svc

kubectl apply -f k8s/configmap-env.yaml
kubectl apply -f k8s/configmap-family.yaml
kubectl apply -f k8s/hpa.yaml

kubectl apply -f k8s/pvc.yaml

kubectl apply -f k8s/statefulset.yaml