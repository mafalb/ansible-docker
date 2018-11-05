# An ansible module for docker [![Build Status](https://travis-ci.com/mafalb/ansible-docker.svg?branch=master)](https://travis-ci.com/mafalb/ansible-docker)

## Basic Usage

```
- hosts: localhost
  roles:
    - role: docker/daemon
```
to install the docker daemon  
or

```
- hosts: localhost
  roles:
    - role: docker/ansible
```
to install the requirements for handling docker images or containers on an ansible node  
e.g. [docker_image](https://docs.ansible.com/ansible/latest/modules/docker_container_module.html#docker-container-module) or  [docker_container](https://docs.ansible.com/ansible/latest/modules/docker_container_module.html#docker-container-module)

## Variables

```
docker_assume_already_installed: false
```
use this to avoid installing docker, e.g. on travis-CI where docker is known to be present in a newer version than the OS provided docker

## License

GPLv3
