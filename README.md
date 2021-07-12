# Redis manifests

This repository keeps kustomize bases for redis, based on [https://github.com/bitnami/charts/tree/master/bitnami/redis](`bitnami/redis`) helm charts.

## Available bases

- `/standalone`: This is the simplest and most common redis set-up you can have, running a single redis instance.

## Updating

```
# Add the repo if you don't have it installed
helm repo add bitnami https://charts.bitnami.com/bitnami

# Or update the repo
helm repo update

helm template bitnami/redis --values ./chart-values/standalone.yaml --name-template redis > ./standalone/redis.yaml
```
