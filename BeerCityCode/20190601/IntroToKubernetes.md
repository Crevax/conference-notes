# An Introduction to Kubernetes by Jason Farrell

## Misc

At its core k8s is a platform for running containers; it has a whole host of tooling to work with resources using k8s.

## Key Concepts

### Cluster

Where everything lives

### Node

Organized compute resources managed by the cluser.

### Pod

The lowest unit; one or more containers carrying out work. They need to be ephemeral, and can be deployed across nodes (which is actually recommended for resialancy).

### Deployment

Defined group of Pods with minimum that need to be running

### Service

Too slow, whoops.

## Resources

(https://kubernetes.io/docs/setup/minikube/)

[Speaker Demo](https://github.com/xximjasonxx/kubedemo)

### Common Tools Used with K8s

- Prometheus (monitoring)
- Rook (storage orchestration)
- Istio (servce mesh and cluster traffic tracking)

### Real World Examples

Tinder (see blog article on Tinder's migration to K8s)
