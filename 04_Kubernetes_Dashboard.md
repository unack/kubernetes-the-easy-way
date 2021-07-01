Kubernetes Dashboard install

```
user@planemaster $ kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/master/aio/deploy/recommended.yaml
```

Dashboard Admin authentication by token
 - Init
```
user@planemaster $ kubectl create serviceaccount dashboard-admin-sa
user@planemaster $ kubectl create clusterrolebinding dashboard-admin-sa --clusterrole=cluster-admin --serviceaccount=default:dashboard-admin-sa
```

 - Get token
```
user@planemaster $ kubectl get secrets
user@planemaster $ kubectl describe secret dashboard-admin-sa-token-qzkg2
```

Dashboard Proxy
 - Init proxy
```
user@planemaster $ kubectl proxy
```
 - Access Dashboard through proxy
```
http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/
```

