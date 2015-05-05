gvillalta99.nvm
===============

Install nvm and Node.js.

This role is an extension of [ahmednuaman/ansible-nvm](https://github.com/ahmednuaman/ansible-nvm)

Installation
------------

`$ ansible-galaxy install gvillalta99.nvm`

Dependencies
------------

On Fedora:

  - git
  - gcc
  - gcc-c++
  - make
  - openssl-devel
  - libselinux-python

On Ubuntu:

  - git
  - curl
  - build-essential
  - libssl-dev

Example Playbook
----------------

    - hosts: servers
      roles:
        - role: nvm
          nvm:
            user: deploy
            version: v0.17.3
            node_version: '0.12'
            packages:
              - grunt-cli
              - bower
              - yo

Requirements
------------

- Tested on Fedora 19
- Tested on Ubuntu 14.04 (Trusty)

License
-------

BSD
