# devskill-k8s-deploy overlay
Kubernetes Workload Deployment Workbench

## Dependencies:
  - [kubectl] 1.21+
  - [kustomize] 4.1.3+
  - [github.com/usrbinkat/devskill-k8s-deploy-base]

### Example kustomize resource modification
  - Source: [kongplugin crd base](https://github.com/usrbinkat/devskill-k8s-deploy-base/tree/main/bases/kongplugin)
  - Overlay: [kongplugin crd kustomization](https://github.com/usrbinkat/devskill-k8s-deploy-overlay)

```sh
kustomize build https://github.com/usrbinkat/devskill-k8s-deploy-overlay
```

[kubectl]:https://kubernetes.io/docs/tasks/tools/install-kubectl-linux
[kustomize]:https://github.com/kubernetes-sigs/kustomize/releases
[github.com/usrbinkat/devskill-k8s-deploy-base]:https://github.com/usrbinkat/devskill-k8s-deploy-base
