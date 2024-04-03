# step configmap
```
1) download conf
curl -o nginx.conf https://github.com/denitiawan/argocd-gitops/blob/main/localhost/concept-2/nginx/nginx-conf/nginx.conf

2) create configmap
kubectl create configmap nginx-config-app-2 --from-file=nginx.conf -n app-2
```

# info
```
[show all configmap]
kubectl get configmaps -n app-2

[delete configmap]
kubectl delete configmap nginx-config-app-2 -n app-2

[Cleanup: Remove the downloaded file]
rm nginx.conf
```
