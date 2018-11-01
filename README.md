# An ansible module for docker [![Build Status](https://travis-ci.com/mafalb/ansible-docker.svg?branch=master)](https://travis-ci.com/mafalb/ansible-docker)

## Basic Usage

```
- hosts: localhost
  roles:
    - role: docker/daemon
```
to install the docker daemon

```
- hosts: localhost
  roles:
    - role: docker/ansible
```
to install the requirements for handling docker images or containers on an ansible node
e.g. [docker_image](https://docs.ansible.com/ansible/latest/modules/docker_container_module.html#docker-container-module) or [docker_container](https://docs.ansible.com/ansible/latest/modules/docker_container_module.html#docker-container-module)


***

## Variables

At this time there are no variables you can use. All configuration is made by the role itself.

## License

GPLv3
