talos
=====

This role bootstraps:
- a containerized Kubernetes cluster
- with one single node running Sidero Talos OS
- with cilium as default CNI.

Requirements
------------

- talosctl
- yq
- kubectl
- helm

Required Role Variables
-----------------------

None

Default Role Variables
----------------------

- `talos_cilium_chart_version`:
- `talos_kube_api_port`:
- `talos_config_dir`:

Dependencies
------------

collections:
  - community.docker
  - kubernetes.core

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
    - name: Create cluster
      ansible.builtin.import_role:
        name: talos
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
