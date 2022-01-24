# k8s-multi-env-kustomize-demo
Deploy your application into multiple environments and increase control over your applications using Kustomize.

This repository demonstrates one application deployed in to both stage and prod environments with differing configurations.

To build both environments:
```
kustomize build apps/my-web-app/overlays/environments/stage > stage.yaml
kustomize build apps/my-web-app/overlays/environments/prod > prod.yaml
```