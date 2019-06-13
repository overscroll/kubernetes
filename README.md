

## Deployments

Get All Deployments:
```
kubectl get deployment
```
Delete Deployments:
```
kubectl delete deployment website
```
Apply a deployment
```
kubectl apply -f strapi/deployment.yaml
```
Scale a deployment
```
kubectl scale deployment strapi --replicas=1
```

```
kubectl rolling-update strapi --image=overscroll/strapi:latest
```


## Services
See all Services 
```
kubectl get services
````



## Debugging

```
kubectl get pod
```
```
kubectl log strapi-66fbdd9594-ftvsz
```
```
kubectl attach strapi-66fbdd9594-ftvsz
```

```
kubectl port-forward service/postgres 5433:5432
```
```
kubectl get services --all-namespaces
```
```
kubectl exec -it strapi-566fc5f6cb-q7js9 -- /bin/sh
```


