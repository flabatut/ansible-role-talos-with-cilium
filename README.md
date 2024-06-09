# Ansible Role to deploy Talos with Cilium

*This is for educational purpose*

This ansible role bootstraps one single node running Sidero Talos OS with cilium as default CNI. Cilium is configured by default with LoadbalancerIP pool and L2 announcement support.

## Requirements

- a machine running talos in maintenance mode

## Getting Started

1. Setup local env:
```
git clone git@github.com:flabatut/ansible-role-talos-with-cilium.git
poetry install
```

2. Get up and running a Talos cluster running as a docker container:

```
task molecule -- create -s docker
```

3. Alternatively, using Tart.run as backend infra:

```
task molecule -- create -s tart
```

4. List available backends (AKA molecule scenarios):

```
task molecule -- list
```

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
