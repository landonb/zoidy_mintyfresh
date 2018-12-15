zoidy_mintyfresh
================

An Ansible role to install packages specific to one Developer's
`Linux Mint 19 ‘Tara’ <https://linuxmint.com/edition.php?id=256>`__
(`Ubuntu 18.04 <http://releases.ubuntu.com/18.04/>`__)
-
`MATE <https://mate-desktop.org/>`__
development machine.

Requirements
------------

A fresh install of Mint.

Example Playbook
----------------

It's simple to run the role from a playbook::

  - hosts: servers
    roles:
       - role: zoidy_mintyfresh

This role needs to become ``root`` to install packages,
so add ``-K`` to be prompted for the password.::

  ansible-playbook path/to/site.yml -K

If you want to restrict what's installed to a specific group, use tags, e.g.,::

  ansible-playbook path/to/site.yml -K --tags install-develop-vim

License
-------

`GPLv3 <LICENSE>`__

