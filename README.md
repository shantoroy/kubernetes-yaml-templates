# Kubernetes Yaml Templates

## Updates from the fork
1. Cleaned the ReadMe
2. Included [common practices](https://github.com/antonputra/tutorials/tree/main/lessons/171) by Antonputra
3. TBD... 

## Notes from Original ReadMe

- **PDF Link:** [kubernetes-yaml-templates.pdf](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/kubernetes-yaml-templates.pdf)
- **Category:** [Cloud](https://cheatsheet.dennyzhang.com/category/cloud/)
- **Blog URL:** [Kubernetes YAML Templates](https://cheatsheet.dennyzhang.com/kubernetes-yaml-templates)
- **Related Posts:**
  - [Kubectl CheatSheet](https://cheatsheet.dennyzhang.com/cheatsheet-kubernetes-A4)
  - [Kubernetes YAML](https://cheatsheet.dennyzhang.com/kubernetes-yaml-templates)
  - [#denny-cheatsheets](https://github.com/topics/denny-cheatsheets)
- **Issues & Contributions:** [File an Issue](https://github.com/dennyzhang/cheatsheet.dennyzhang.com/issues) | [Star the Repo](https://github.com/dennyzhang/cheatsheet.dennyzhang.com)

## Pod

| Yaml | Summary |
|-------------------------------|------------------------------------------------|
| [pod/pod-dummy.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/pod/pod-dummy.yaml) | Start a dummy pod with a dead sleep loop |
| [pod/pod-nginx.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/pod/pod-nginx.yaml) | Start a pod of sample app (nginx) |
| [pod/pod-initcontainer-sysctl.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/pod/pod-initcontainer-sysctl.yaml) | Use initContainer to run sysctl when starting a Pod |
| [pod/pod-healthcheck-nginx.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/pod/pod-healthcheck-nginx.yaml) | Start pod with TCP and HTTP healthcheck |
| [pod/pod-secrets.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/pod/pod-secrets.yaml) | Use secrets as volumes or environment variables |
| [pod/pod-gitclone.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/pod/pod-gitclone.yaml) | Use initContainer as sidecar to web host a git repo |
| [pod/pod-hostaliases.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/pod/pod-hostaliases.yaml) | Add alias to /etc/hosts |
| [pod/pod-serviceaccount.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/pod/pod-serviceaccount.yaml) | Start pod with serviceaccount |
| [pod/pod-handlers.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/pod/pod-handlers.yaml) | Pod's events whenever it starts or stops |

Reference: [Kubectl CheatSheet](https://cheatsheet.dennyzhang.com/cheatsheet-kubernetes-A4)

## Volume

| Yaml | Summary |
|--------------------------------------|----------------------------------------------------|
| [volume/volume-manual-pv.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/volume/volume-manual-pv.yaml) | Create PV first, then PVC |
| [volume/volume-mount-localpath.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/volume/volume-mount-localpath.yaml) | Mount a local folder to pods |
| [volume/volume-emptydir.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/volume/volume-emptydir.yaml) | Create an empty folder and mount to pods |
| [volume/volume-ebs.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/volume/volume-ebs.yaml) | Mount EBS volume to a pod in the same AZ |
| [volume/volume-nfs.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/volume/volume-nfs.yaml) | Create NFS PV |
| [volume/volume-gcePersistentDisk.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/volume/volume-gcePersistentDisk.yaml) | Mount GCE disk to a pod |
| [volume/volume-digitalocean.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/volume/volume-digitalocean.yaml) | Create DigitalOcean volume for Kubernetes cluster |

Reference: [Kubectl CheatSheet](https://cheatsheet.dennyzhang.com/cheatsheet-kubernetes-A4) | [Volumes Examples](https://github.com/kubernetes/examples/tree/master/staging/volumes)

## Service

| Yaml | Summary |
|---------------------------------|-------------------------------|
| [service/service-loadbalancer.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/service/service-loadbalancer.yaml) | LoadBalancer Service |
| [service/service-nodeport.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/service/service-nodeport.yaml) | NodePort Service |
| [service/service-ingress.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/service/service-ingress.yaml) | Ingress Service |
| [service/service-clusterip-nginx.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/service/service-clusterip-nginx.yaml) | ClusterIP Service for nginx |
| [service/service-cassandra.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/service/service-cassandra.yaml) | Cassandra Service |

Reference: [Kubectl CheatSheet](https://cheatsheet.dennyzhang.com/cheatsheet-kubernetes-A4)

## ConfigMap & Environments

| Yaml | Summary |
|----------------------------------|------------------------------------------|
| [config/pod-configmap.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/config/pod-configmap.yaml) | Create ConfigMap and use as pod volume |
| [config/pod-environment-var.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/config/pod-environment-var.yaml) | Pass environment variables to a pod |
| [config/pod-env-metada.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/config/pod-env-metada.yaml) | Expose metadata to pods |
| [config/configmap-plaintext.yaml](https://github.com/dennyzhang/kubernetes-yaml-templates/blob/master/config/configmap-plaintext.yaml) | Define ConfigMap with plain text |



