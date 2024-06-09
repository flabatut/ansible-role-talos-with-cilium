# Ansible Role to deploy Talos in Tart

*This is for educational purpose*

This ansible role bootstraps:
- a containerized Kubernetes cluster
- with one single node running Sidero Talos OS
- with cilium as default CNI.

## Requirements

- [tart](https://tart.run/)
- [poetry](https://python-poetry.org/docs/basic-usage/)

## Getting Started

- Start devcontainer
- Create the cluster: `molecule create`
- After a few minutes, your `kubeconfig` should be ready to query your freshly created cluster.
- Destroy the cluster: `molecule destroy`

## Rational

- doing it for fun
- learn and understand the steps involved in `talosctl cluster create`
- customize talos cluster with only one single node
- tight integration with molecule framework
- get familiar with cilium and talos

## References

- https://www.talos.dev/v1.8/talos-guides/install/local-platforms/docker/
- https://ansible.readthedocs.io/projects/molecule/getting-started/
- https://cilium.io/
