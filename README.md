# containerd-guide

list all namespaces:
```bash
ctr ns ls
```

list all images in `k8s.io` namespace:
```bash
ctr -n k8s.io i ls -q
```

list all containers in `k8s.io` namespace:
```bash
ctr -n k8s.io c ls -q
```

pull container image:
```bash
ctr i pull docker.io/library/busybox:latest
```

run container:
```bash
ctr run --rm docker.io/library/busybox:latest 1
```

remove image in `k8s.io` namespace:
```bash
ctr -n k8s.io i rm docker.io/library/nginx:alpine
```
