
Common Gotchas
==============

VIM Arrow Keys Don't Work
-------------------------

You may notice that by default, VIM's arrow keys don't work on your computer. To fix this, add the following to your ``~/.vimrc``::

    $ cat ~/.vimrc
    set term=builtin_ansi