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

NOTE: Unfortunately this is currently not working. See this [issue](<https://github.com/kubernetes-sigs/kustomize/issues/4658>)

Deploy to dev

```shell
cd project-2
kubectl kustomize overlays/dev --enable-helm
```

Deploy to prod

```shell
cd project-2
kubectl kustomize overlays/prod --enable-helm
```
