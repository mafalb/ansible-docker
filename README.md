# An ansible module for docker [![Build Status](https://travis-ci.com/mafalb/ansible-docker.svg?branch=master)](https://travis-ci.com/mafalb/ansible-docker)

## Basic Usage

To install docker:
```
- hosts: localhost
  roles:
    - role: docker/daemon
```

If you want to build docker images on an ansible node:
```
- hosts: localhost
  roles:
    - role: docker/ansible
```

## Variables

```
docker_package: ''
```

Per default the name of the package to be installed is set automatically per OS. You can override the name of the package manually, e.g. you can force installation of docker-ce instead of the OS docker by setting

```
docker_package: docker-ce
```

You don't have to do this if running on travis-CI. The role does detect travis-CI and overrules the default OS docker_package name appropiatly to docker-ce

License
-------

GPLv3
