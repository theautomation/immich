# immich

![GitHub repo size](https://img.shields.io/github/repo-size/theautomation/immich?logo=Github)
![GitHub commit activity](https://img.shields.io/github/commit-activity/y/theautomation/immich?logo=github)
![GitHub last commit (branch)](https://img.shields.io/github/last-commit/theautomation/immich/main?logo=github)

Application running in Kubernetes <img src="https://github.com/theautomation/kubernetes-gitops/blob/main/assets/img/k8s.png?raw=true" alt="K8s" style="height: 40px; width:40px;"/>

Forked from the orginal repository https://github.com/immich-app/immich. This repo only contains a yaml manifest (I dont like Helm) for a deployment on Kubernetes. I use truenas as storage backend and Bitnami Sealedsecret to encrypt the secrets in the yaml. 

Storage template
```
{{y}}/{{MM}}/{{y}}{{MM}}{{dd}}_{{hh}}{{mm}}{{ss}}_{{filetype}}_{{filename}}
```