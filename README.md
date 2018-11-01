# An ansible module for docker [![Build Status](https://travis-ci.com/mafalb/ansible-docker.svg?branch=master)](https://travis-ci.com/mafalb/ansible-docker)

## Basic Usage

```
- hosts: localhost
  roles:
    - role: docker/daemon
```
to install the docker daemon
***
```
- hosts: localhost
  roles:
    - role: docker/ansible
```
if you want to build docker images on an ansible node to install node requirements for docker.
***
## Variables

At this time there are no variables you can use. All configuration is made by the role itself.

## License

GPLv3
