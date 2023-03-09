## Workshop with Kubernetes with minikube

### Start minikube
```
$minikube start --driver=docker --alsologtostderr
$minikube dashboard --url
```
### Working with kubectl
```
$kubectl get node
NAME       STATUS   ROLES           AGE     VERSION
minikube   Ready    control-plane   5h41m   v1.26.1
```

Deploy
```
$kubectl apply -f backend.yml
$kubectl apply -f frontend.yml

$kubectl get pod
kubectl describe pod

$kubectl get deployment
$kubectl get service
```

Access to frontend
```
$minikube service react-nginx-service --url
```