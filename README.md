# K8s Object Deployment Workbench

## Example with kustomize overlays
### Dependencies:
  - [kustomize] 4.1.3+ / or / [kubectl] 1.21+
  - Source: [kongplugin crd base](https://github.com/usrbinkat/devskill-k8s-deploy-base/tree/main/bases/kongplugin)
  - Overlay: [kongplugin crd kustomization](https://github.com/usrbinkat/devskill-k8s-deploy-overlay)

```sh
kustomize build https://github.com/usrbinkat/devskill-k8s-deploy-overlay?ref=main
```

[kubectl]:https://kubernetes.io/docs/tasks/tools/install-kubectl-linux
[kustomize]:https://github.com/kubernetes-sigs/kustomize/releases
[github.com/usrbinkat/devskill-k8s-deploy-base]:https://github.com/usrbinkat/devskill-k8s-deploy-base

---
## Example with Helm templating engine
### Dependencies:
  - git
  - [helm] 3.6+
  - Source: [kongplugin crd base](https://github.com/usrbinkat/devskill-k8s-deploy-base/tree/main/helm)

```sh
git clone https://github.com/usrbinkat/devskill-k8s-deploy-base /tmp/devskill
cd /tmp/devskill/helm
helm template test-api ./ > rendered.yaml
```