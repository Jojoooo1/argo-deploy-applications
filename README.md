# Argo applications personal labs

## applications

## ArgoCD Folders organization

### Base

- **base/applications-data**: Contains k8s observability applications

### Overlay

Environments folders that inherit from base folder. It uses [kustomize](https://github.com/kubernetes-sigs/kustomize) to allow environment based customization.
