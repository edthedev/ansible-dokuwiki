ansible-dokuwiki
================

Ansible script to install Dokuwiki, stolen from the Dokuwiki_Wiki_.

.. _Dokuwiki_Wiki: https://www.dokuwiki.org/install:ansible

To run it:

1. Install Ansible on your local computer.

2. Setup a public SSH key to access your remote computer.

3. Clone this repository to your local computer.

4. Update `dokuwiki.yml` with your remote computer's hostname and user.

5. Run the ansible playbook.::

    ansible-playbook --skip-tags=after_installation dokuwiki.yml
