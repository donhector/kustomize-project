# Kustomize playground

## project-1

Deploy to dev

```shell
cd project-1
kubectl kustomize overlays/dev | kubectl apply -f -
```

Deploy to prod

```shell
cd project-1
kubectl kustomize overlays/prod | kubectl apply -f -
```

## project-2

Deploy to dev

```shell
cd project-2
kubectl kustomize --enable-helm
```
