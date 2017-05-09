
Common Gotchas
==============

VIM Arrow Keys Don't Work
-------------------------

You may notice that by default, VIM's arrow keys don't work on your computer. To fix this, add the following to your ``~/.vimrc``::

    $ cat ~/.vimrc
    set term=builtin_ansi

Sudo 'Unable to Resolve Host' Warning
-------------------------------------

You may notice that every time you run ``sudo something``, your system complains that it cannot resolve it's own hostname, but then continues on anyway. To fix this annoyance, you need to add your system's hostname to ``/etc/hosts``::

    $ cat /etc/hosts
    127.0.0.1 localhost
    127.0.0.1 nova
    ...

Here, my machine is called 'nova'. 

Connecting to the Linux subsystem via SSH
-----------------------------------------

In order to be able to ssh into your Linux subsystem instance follow the steps outlined by Master Azazel in this `thread: <https://superuser.com/a/1114162>`_

1. ``sudo apt-get remove openssh-server``
2. ``sudo apt-get install openssh-server``
3. ``sudo nano /etc/ssh/sshd_config`` and disallow root login by setting ``PermitRootLogin no``
4. Then add a line beneath it that says: ``AllowUsers yourusername`` and make sure ``PasswordAuthentication`` is set to ``yes`` if you want to login using a password.
5. Disable privilege separation by adding/modifying : ``UsePrivilegeSeparation no``
6. ``sudo service ssh --full-restart``
7. Connect to your Linux subsystem from Windows using a ssh client like PuTTY.
