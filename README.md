# Deployment

## Pre-re

Make sure you have Docker installed in your machine with kubernetes enabled.

## Steps

1. Create namespace

```bash
kubectl create ns demo
```


2. Intall ingress-nginx dependencies.

```bash
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v0.41.0/deploy/static/provider/cloud/deploy.yaml
```

3. Configure the ingress-nginx and apply.

```bash
kubectl apply -f ingress-nginx.yaml -n demo