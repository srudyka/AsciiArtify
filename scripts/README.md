# Kubectl plugin: kubectl-pod-top

### This kubectl plugin retrieves and displays the CPU and memory usage of pods in a specified Kubernetes namespace.


### Install: 

Copy `kubectl-pod-top` into `/usr/local/bin/`

Usage:


`kubectl pod top <namespace>`

Example of output:

1.

>$kubectl pod top

>Resource          | Namespace             | Name            | CPU          |        Memory

>pod                | default             | nginx               | 0m         | 3Mi

2.
 
 >$kubectl pod top kube-system
 
>Resource          | Namespace             | Name            | CPU          |        Memory

>pod                | kube-system             | coredns-66bc5c9577-qc67b               | 5m         | 84Mi

>pod                | kube-system             | etcd-minikube               | 48m         | 372Mi

>pod                | kube-system             | kube-apiserver-minikube               | 90m         | 355Mi

>pod                | kube-system             | kube-controller-manager-minikube               | 33m         | 116Mi

>pod                | kube-system             | kube-proxy-mxfwl               | 1m         | 61Mi

>pod                | kube-system             | kube-scheduler-minikube               | 21m         | 68Mi

>pod                | kube-system             | metrics-server-8cc67c988-stgkh               | 7m         | 18Mi

>pod                | kube-system             | storage-provisioner               | 4m         | 17Mi


