# Helm chart for deploying Navidrome to K8s

Bare bones helm chart for deploying Navidrome to k8s. 

Expects to use NFS for 2 PVs. Chart will create the PV and PVCs so values under `persistenVolume` must be set correctly.

see [values.yaml](navidrome/values.yaml) for configurations.

Install using Helm v3:

```
helm repo add flipenergy https://flipenergy.github.io/k8s-homelab/
helm install my-release flipenergy/navidrome
```
