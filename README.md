# K8s infra with ArgoCD 🐙☸️

Multi-tenancy, local setup, bootstrap script and more.

## Getting started 🚀

```sh
# start local cluster (https://kind.sigs.k8s.io/)
kind create cluster --wait 5m --config=./scripts/kind/kind-config.yaml ## Ignore if you already have a cluster setup

# bootstrap argocd on the cluster
./scripts/bootstrap.sh --cluster=local
# follow the instructions to get the argocd password and the URL or make an alias
```

## Commands 💻

```sh
./scripts/bootstrap.sh --help

./scripts/lint-helm.sh
./scripts/lint-helm-stagged.sh
```

Note: adapt the structure to your org... #ConwaysLaw
