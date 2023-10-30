# [enpass](#enpass)

Install the Enpass password manager on your system.

|GitHub|GitLab|Quality|Downloads|Version|Issues|Pull Requests|
|------|------|-------|---------|-------|------|-------------|
|[![github](https://github.com/buluma/ansible-role-enpass/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-enpass/actions)|[![gitlab](https://gitlab.com/shadowwalker/ansible-role-enpass/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/ansible-role-enpass)|[![quality](https://img.shields.io/ansible/quality/)](https://galaxy.ansible.com/buluma/enpass)|[![downloads](https://img.shields.io/ansible/role/d/)](https://galaxy.ansible.com/buluma/enpass)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-enpass.svg)](https://github.com/buluma/ansible-role-enpass/releases/)|[![Issues](https://img.shields.io/github/issues/buluma/ansible-role-enpass.svg)](https://github.com/buluma/ansible-role-enpass/issues/)|[![PullRequests](https://img.shields.io/github/issues-pr-closed-raw/buluma/ansible-role-enpass.svg)](https://github.com/buluma/ansible-role-enpass/pulls/)|

## [Example Playbook](#example-playbook)

This example is taken from [`molecule/default/converge.yml`](https://github.com/buluma/ansible-role-enpass/blob/master/molecule/default/converge.yml) and is tested on each push, pull request and release.

```yaml
---
- name: Converge
  hosts: all
  become: yes
  gather_facts: yes

  roles:
    - role: buluma.enpass
```

The machine needs to be prepared. In CI this is done using [`molecule/default/prepare.yml`](https://github.com/buluma/ansible-role-enpass/blob/master/molecule/default/prepare.yml):

```yaml
---
- name: Prepare
  hosts: all
  become: yes
  gather_facts: no

  roles:
    - role: robertdebock.bootstrap
```

Also see a [full explanation and example](https://buluma.github.io/how-to-use-these-roles.html) on how to use these roles.

## [Role Variables](#role-variables)

The default values for the variables are set in [`defaults/main.yml`](https://github.com/buluma/ansible-role-enpass/blob/master/defaults/main.yml):

```yaml
---
# defaults file for enpass
```

## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-enpass/blob/master/requirements.txt).

## [State of used roles](#state-of-used-roles)

The following roles are used to prepare a system. You can prepare your system in another way.

| Requirement | GitHub | GitLab |
|-------------|--------|--------|
|[robertdebock.bootstrap](https://galaxy.ansible.com/buluma/robertdebock.bootstrap)|[![Build Status GitHub](https://github.com/buluma/robertdebock.bootstrap/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/robertdebock.bootstrap/actions)|[![Build Status GitLab](https://gitlab.com/shadowwalker/robertdebock.bootstrap/badges/master/pipeline.svg)](https://gitlab.com/shadowwalker/robertdebock.bootstrap)|

## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.github.io/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-enpass/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|[Debian](https://hub.docker.com/repository/docker/buluma/debian/general)|all|
|[EL](https://hub.docker.com/repository/docker/buluma/enterpriselinux/general)|all|
|[Fedora](https://hub.docker.com/repository/docker/buluma/fedora/general)|all|
|[opensuse](https://hub.docker.com/repository/docker/buluma/opensuse/general)|all|
|[Ubuntu](https://hub.docker.com/repository/docker/buluma/ubuntu/general)|all|

The minimum version of Ansible required is 2.12, tests have been done to:

- The previous version.
- The current version.
- The development version.

If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-enpass/issues)

## [Changelog](#changelog)

[Role History](https://github.com/buluma/ansible-role-enpass/blob/master/CHANGELOG.md)

## [License](#license)

[Apache-2.0](https://github.com/buluma/ansible-role-enpass/blob/master/LICENSE).

## [Author Information](#author-information)

[robertdebock](https://buluma.github.io/)

Please consider [sponsoring me](https://github.com/sponsors/buluma).

### [Special Thanks](#special-thanks)

Template inspired by [Robert de Bock](https://github.com/robertdebock)
