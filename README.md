# jenkins-k8s
Host Jenkins in Kubernetes with Helm, Argo CD


How to use:

1. Configure and install ArgoCD in your K8S Cluster.
   ```
   kubectl create namespace argocd
   kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
   ```

2. Configure ArgoCD to use this repository with path 
helm/charts/jenkins.

![alt text](https://github.com/jerrysf2009/jenkins-k8s/blob/main/pic/argocd.jpg?raw=true)

Note:

When using minikube, get the Jenkins server URL using: 

```
minikube service --url jenkins-server -n jenkins
```


