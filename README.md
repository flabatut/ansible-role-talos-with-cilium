# Ansible Role to deploy Talos with Cilium

*This is for educational purpose*

This ansible role bootstraps one single node running Sidero Talos OS with cilium as default CNI. Cilium is configured by default with LoadbalancerIP pool and L2 announcement support.

## Requirements

- a machine running talos in maintenance mode

## Testing

```
poetry shell
molecule test
```
> molecule list to get available backends supported (ie: docker, tart,...)

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
