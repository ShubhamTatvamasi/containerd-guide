# containerd-guide

list all namespaces
```
ctr ns ls
```

list all images in `k8s.io` namespace
```bash
ctr -n k8s.io i ls -q
```

list all containers in `k8s.io` namespace
```bash
ctr -n k8s.io c ls -q
```
