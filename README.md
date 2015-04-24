nvm
===

Install nvm and Node.js.

This role is an extension of [leonidas/ansible-nvm role](https://github.com/leonidas/ansible-nvm).

Installation
------------

`$ ansible-galaxy install gvillalta99.google_chrome`

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
            node_version: '0.10'
            packages:
              - bower
              - karma

Requirements
------------

- Tested on Fedora 19

License
-------

BSD
