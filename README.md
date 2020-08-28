Buildah
=========
[![Build Status](https://travis-ci.org/islander/ansible-role-buildah.svg?branch=master)](https://travis-ci.org/islander/ansible-role-buildah)

A role to install [buildah][1] container image build tool.


Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

```
buildah_repo_url: "deb https://download.opensuse.org/repositories/devel:/kubic:/libcontainers:/stable/xUbuntu_{{ ansible_distribution_version }}/ /"
buildah_sources_list: "/etc/apt/sources.list.d/devel:kubic:libcontainers:stable.list"
buildah_key_url: "https://download.opensuse.org/repositories/devel:/kubic:/libcontainers:/stable/xUbuntu_{{ ansible_distribution_version }}/Release.key"
```

Example Playbook
----------------
Install role from galaxy: `ansible-galaxy install islander.buildah`

    - hosts: servers
      roles:
         - islander.buildah

License
-------

BSD

Author Information
------------------

This role was created by [kiba][2]

[1]: https://buildah.io
[2]: https://kiba.io
