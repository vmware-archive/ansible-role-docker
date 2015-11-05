# ansible-role-docker

[Ansible](https://github.com/ansible/ansible) role for adding
and managing Docker Engine services.

## Requirements

None known.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    ubuntu_release: trusty

Ubuntu version to use for aptitude package repositories.

    docker_opes: (undefined)

Docker options to add to the docker daemon run command. See defaults/main.yml.

## Example playbook

```
---
- hosts: dockers
  sudo: True
  roles:
    - docker
  vars:
    docker_opts: "--dns 8.8.8.8 --dns 8.8.4.4"
```

# License and Copyright

Copyright 2015 VMware, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

## Author Information

This role was created in 2015 by [Tom Hite / VMware](http://www.vmware.com/).
