![Status](https://travis-ci.org/asg1612/ansible-role-docker.svg?branch=master) [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/1849/badge)](https://bestpractices.coreinfrastructure.org/projects/1849)
![](https://github.com/actions/asg1612/workflows/.github/workflows/main.yml/badge.svg)
Role Docker
=========

This role is for install Docker system. Testing with molecule

Requirements
------------

None

Role Variables
--------------
**daemon_json**: Dictionary with daemon.json options
**docker_version**: Docker version ej: docker_version: 18.03.*

Dependencies
------------

None


Example Playbook
----------------

    - hosts: servers
      vars:
        daemon_json:
          registry-mirrors:
            - http://example.com:5001
          insecure-registries:
            - example.com:5000
          dns:
            - 8.8.8.8
      roles:
         - { role: asg1612.ansible-role-docker }


License
-------

[GNU General Public License v 3.0](https://www.gnu.org/licenses/gpl-3.0)


Author Information
------------------

Andrés Sánchez García

twitter: @asg1612

e-mail: asg1612@gmail.com

linkedin: https://www.linkedin.com/in/asg1612/

website: http://andressaga.es/
