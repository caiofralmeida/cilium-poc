# Cilium PoC

## Creating the Kuberneter cluster

The command bellow creates a new kind cluster with 1 control plane and 3 workers nodes, disabling the default CNI plugin.

```sh
kind create cluster --name cilium --config=kind-config.yaml
```

The result should be:

```sh
Creating cluster "cilium" ...
 ✓ Ensuring node image (kindest/node:v1.21.1) 🖼
 ✓ Preparing nodes 📦 📦 📦 📦  
 ✓ Writing configuration 📜 
 ✓ Starting control-plane 🕹️ 
 ✓ Installing StorageClass 💾 
 ✓ Joining worker nodes 🚜 
Set kubectl context to "kind-cilium"
You can now use your cluster with:

kubectl cluster-info --context kind-cilium

Not sure what to do next? 😅  Check out https://kind.sigs.k8s.io/docs/user/quick-start/
```