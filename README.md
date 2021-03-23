# jenkins-k8s
Host Jenkins Server in Kubernetes with Helm, Argo CD


<h2>How to use:</h2>

1. Configure and install ArgoCD in your K8S Cluster.
   ```
   kubectl create namespace argocd
   kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
   ```

2. Configure ArgoCD to use this repository with path 
helm/charts/jenkins.

![](./pic/argocd1.jpg)

<h2>How it is looks like:</h2>

![](./pic/argocd.jpg)

<h2>Note:</h2>

When using minikube:

Get the Jenkins server URL using: 

```
minikube service --url jenkins-server -n jenkins
```

Enable ingress for minikube:

```
minikube addons enable ingress
```

