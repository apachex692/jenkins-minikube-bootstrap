# Jenkins Bootstrap on minikube

- **Author:** Apache X692
- **Created on:** 12/12/2024

This repository contains manifests to provision Jenkins server on minikube. Ensure you do the following before running the manifest:

```sh
kubectl create namespace jenkins
```

Now, execute the commands in the following order:

```sh
kubectl apply -f ./sa.yaml
kubectl apply -f ./volume.yaml
kubectl apply -f ./deploy.yaml
kubectl apply -f ./svc.yaml
```
