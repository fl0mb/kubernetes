# Kubernetes (K8s)

[![Go Report Card](https://goreportcard.com/badge/github.com/kubernetes/kubernetes)](https://goreportcard.com/report/github.com/kubernetes/kubernetes) ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/kubernetes/kubernetes?sort=semver)

<img src="https://github.com/kubernetes/kubernetes/raw/master/logo/logo.png" width="100">


Kubernetes fork to build custom `kubectl` which adds a custom header and allows authentication via unencrypted HTTP connections. Mainly a test to exploit Tekton dashboard proxying behavior.

Build:
```bash
git clone https://github.com/fl0mb/kubernetes.git
go build -o k-test cmd/kubectl/kubectl.go
```

Example use:
```bash
./kubectl exec -it pod --server='http://<tekton-dashboard>:9097' --token=$token -- sh     
```
----

Kubernetes, also known as K8s, is an open source system for managing [containerized applications]
across multiple hosts. It provides basic mechanisms for the deployment, maintenance,
and scaling of applications.

Kubernetes builds upon a decade and a half of experience at Google running
production workloads at scale using a system called [Borg],
combined with best-of-breed ideas and practices from the community.

Kubernetes is hosted by the Cloud Native Computing Foundation ([CNCF]).
If your company wants to help shape the evolution of
technologies that are container-packaged, dynamically scheduled,
and microservices-oriented, consider joining the CNCF.
For details about who's involved and how Kubernetes plays a role,
read the CNCF [announcement].

----
