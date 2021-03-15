# jenkins-k8s
Host Jenkins in Kubernetes with Helm, Argo CD


How to use:

1. Configure and install ArgoCD in your K8S Cluster.
2. Configure ArgoCD to use this repository with path 
helm/charts/jenkins.

Note:

When using minikube, get the Jenkins server URL using: 

```
minikube service --url jenkins-server -n jenkins
```


