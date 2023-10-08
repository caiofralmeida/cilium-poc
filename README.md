# Cilium PoC

## Creating the Kuberneter cluster

The command bellow creates a new kind cluster with 1 control plane and 3 workers nodes, disabling the default CNI plugin.

```sh
kind create cluster --name cilium --config=kind-config.yaml
```
