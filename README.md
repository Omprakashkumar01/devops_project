#DevOps project


```
eksctl create cluster --name devopsproj
```
```

```
```
kubectl create namespace argocd
```
```
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
```
```
kubectl config set-context --current --namespace=argocd
```
```
https://github.com/argoproj/argo-cd/releases
```
```
argocd login --core
```
```

argocd admin initial-password -n argocd
```

```
kubectl port-forward svc/argocd-server -n argocd 8080:443
```


```
git init
git add README.md
git commit -m "first commit"
git branch -M master
git remote add origin https://github.com/Omprakashkumar01/devops_project.git
git push -u origin master
```
```
curl https://raw.githubusercontent.com/Omprakashkumar01/devops_project/refs/heads/main/bookinfo.yaml  -o bookinfo.yaml
```

```
git add .
git commit -m first .
git push
```
```
kubectl get pods -n default
```
```
kubectl port-forward  svc/productpage  -n default  80:9080
```

http://127.0.0.1/productpage



```


istioctl  install --set profile=demo
```
```
kubectl get pods -n istio-system
```
```
kubectl get svc  -n istio-system
```
```
kubectl label namespace default  istio-injection=enabled
```
```

kubectl delete pods  --all -n default
```
```
kubectl get pods -n default
```
```
kubectl apply -f bookinfo-gateway.yaml
```
```
cd "C:\Users\omjsr\Downloads\istio-1.24.2-win-amd64 (1)\istio-1.24.2\samples"
```
```
kubectl.exe apply -f addons/
```
```
kubectl get pods -n istio-system
```

```
kubectl get svc -n istio-system
```
```
kubectl get gateway -n default
```
```
kubectl get vs -n default
```
```
helm repo add kiali https://kiali.org/helm-charts
helm repo update
```

```
kubectl port-forward -n istio-system svc/kiali 20001:20001
```
```
kubectl port-forward -n istio-system svc/prometheus 9090:9090
```
```
kubectl port-forward -n istio-system svc/grafana 3000:3000
```














