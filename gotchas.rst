
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