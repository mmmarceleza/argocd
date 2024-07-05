# Openshift IaC

## Instalação do Argo CD com Helm

Instalação do Argo CD:

```bash
helm upgrade --install argo-cd argo-cd \
    -n argo-cd --create-namespace \
    --repo=https://argoproj.github.io/argo-helm \
    --version=7.3.4 \
    -f https://raw.githubusercontent.com/mmmarceleza/arogcd/main/argocd/values.yaml
```

## Instalação das aplicações do repositório

```bash
kubectl apply -f https://raw.githubusercontent.com/mmmarceleza/argocd/main/clusters/hml/cluster-hml-application.yaml
```
