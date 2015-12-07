ansible-docker-consul (**NOT WORKING YET**)
=========

Ansible role for bootstrapping a Docker-based Consul cluster. Currently uses [`gliderlabs/consul:legacy`](https://hub.docker.com/r/gliderlabs/consul/) (might extend this to `gliderlabs/consul:latest` in the future.)

Requirements
------------

Dependencies of the [docker module](http://docs.ansible.com/ansible/docker_module.html), which are presently:
* python >= 2.6
* docker-py >= 0.3.0
* The docker server >= 0.10.0

Role Variables
--------------

TODO: A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

TODO: A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

TODO: Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

Vagrant test
------------

First, install playbook dependencies by running

```
sudo ansible-galaxy install -r requirements.yml # --force
```

Then bring up the vagrant hosts and run the plays against them

```
vagrant up
```

To bring the machines up and run the Ansible plays in _separate steps_ (useful for debugging/developing the role)

```
vagrant up --no-provision
```

Afterwards,

```
vagrant provision
```

License
-------

BSD

Author Information
------------------

[Shujon Mollah](https://github.com/smoll) (@smoll)
