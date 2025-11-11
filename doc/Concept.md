# Comparison of tools for managing local Kubernetes deployments for local development in AsciiArtify


## list of tools 

* minikube : https://minikube.sigs.k8s.io/docs/
* kind : https://kind.sigs.k8s.io
* k3d : https://k3d.io/stable/

### Minikube 
minikube is local Kubernetes, focusing on making it easy to learn and develop for Kubernetes.

All you need is Docker (or similarly compatible) container or a Virtual Machine environment, and Kubernetes is a single command away: `minikube start`
OS: Linux, OSX, Windows
Arh: x86, ARM64
Supported Container or VM managers: Docker, QEMU, Hyperkit, Hyper-V, KVM, Parallels, Podman, VirtualBox, or VMware Fusion/Workstation
Automation: via shell scripts
Additional functions: dashboard with metrics


### kind
kind is a tool for running local Kubernetes clusters using Docker container “nodes”.
kind was primarily designed for testing Kubernetes itself, but may be used for local development or CI.
OS: Linux, OSX, Windows
Arh: x86, ARM64
Supported Container or VM managers: containerd(Docker) with experimental support for podman.
Automation: via shell scripts


### k3d
k3d is a lightweight wrapper to run k3s (Rancher Lab’s minimal Kubernetes distribution) in docker.

k3d makes it very easy to create single- and multi-node k3s clusters in docker, e.g. for local development on Kubernetes.
OS: Linux
Arh: x86, ARM64
Supported Container or VM managers: containerd(Docker),  Podman.
Automation: via shell scripts

## Considerations

Considering the maturity of Minikube as such: 

* availability for  many OS, 
* possibility to use Podman (which helps to mitigate future licensing issues),  
* functionality can be extended with the `minikube addons` feature 
* available the Kubernetes management and metric dashboards out of the box 
 
 I suggest starting to implement Minikube for local development of AsciiArtify developers.
  

Demo: ![](minikube.gif)
Demo link: [https://asciinema.org/a/F7IHr7ijxw56ZhAxT2YlangUX](https://asciinema.org/a/F7IHr7ijxw56ZhAxT2YlangUX)
