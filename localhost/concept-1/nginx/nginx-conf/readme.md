# download conf
curl -o nginx.conf https://github.com/denitiawan/argocd-nginx/blob/main/nginx-conf/nginx.conf

# show all configmap
kubectl get configmaps -n my-application

# delete configmap
kubectl delete configmap nginx-config -n my-application

# create configmap
kubectl create configmap nginx-config --from-file=nginx.conf -n my-application

# Cleanup: Remove the downloaded file
rm nginx.conf

