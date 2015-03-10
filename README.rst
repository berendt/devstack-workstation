devstack-workstation
====================

:code:`devstack-workstation` is an `Ansible playbook <https://github.com/ansible/ansible>`_
to bootstrap a `Devstack <http://docs.openstack.org/developer/devstack/>`_ development environment.

Requirements
------------

A standard `Fedora 21 workstation installation <https://getfedora.org/en/workstation/download/>`_
on a bare-metal system (e.g. a 2nd workstation or a Laptop).

Preparation
-----------

Enable passwordless :code:`sudo` for the :code:`wheel` group in the :code:`/etc/sudoers` configuration file.

.. code::

    ## Allows people in group wheel to run all commands
    # %wheel  ALL=(ALL)       ALL

    ## Same thing without a password
    %wheel        ALL=(ALL)       NOPASSWD: ALL

Installation
------------

.. code::

    $ git clone git@github.com:berendt/devstack-workstation.git
    $ cd devstack-workstation
    $ ./run.sh

Initialization
--------------

.. code::

    $ cd ~/devstack
    $ ./stack.sh
