ansible-dokuwiki
================

Everything is Perl locale pain.

Ansible script to install Dokuwiki, stolen from the Dokuwiki_Wiki_.

.. _Dokuwiki_Wiki: https://www.dokuwiki.org/install:ansible

To run it:

1. Install Ansible on your local computer.

2. Setup a public SSH key to access your remote computer.

3. Clone this repository to your local computer.

4. Update `dokuwiki.yml` with your remote computer's hostname and user.

5. Set the locale on the remote computer.::

   ssh myhostname.example.net
   dpkg-reconfigure locales

6. Run the ansible playbook.::

    ansible-playbook --skip-tags=after_installation dokuwiki.yml

7. Visit the install URL.::

   TODO: Document expected install URL on localhost 8080

8. Run the hardening playbook to close it out.::

   TODO: Split the hardening command into a separate playbook to simplify commands.

