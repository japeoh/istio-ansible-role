# Istio Ansible Role

Installs [Istio](https://istio.io/)

## Variables

| Variable        | Description                             | Default Value |
|-----------------|-----------------------------------------|---|
istio_base_dir    | Where to create the download directory  | ~/tools
istio_install_dir | Where to install `istoctl`              | ~/bin
istio_version     | The version of istio to download        | 1.5.1
istio_checksum    | The checksum for the downloaded archive | sha256:cbaf9c76a75e2585bd3444e96bf64c29b31165981a4dc4a24faf7a34d9f9de01

## Example Playbook

```yaml
- hosts: localhost
  become: yes
  roles:
    - role: japeoh.istio
      vars:
        istio_install_dir: /usr/local/bin
```

## License

GPLv3

##  Development

See [here](https://github.com/japeoh/ansible-role-development) for setup.
