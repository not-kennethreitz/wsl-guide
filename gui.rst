GUI Applications
================

Step 1: Installing an X Server
------------------------------

In order to run GUI applications in WSL, you need to first install an X Server on your Windows machine. 
I recommend installing `Xming <https://sourceforge.net/projects/xming/>`_. 

Step 2: Set DISPLAY Environment Variable
----------------------------------------

Next, you have to tell your WSL environment to use the X Server by setting the ``DISPLAY`` environment variable. 

I added the following to my ``~/.bashrc``::

    export DISPLAY=:0


