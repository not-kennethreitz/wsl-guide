Updating WSL
============

Updating Packages in WSL
------------------------

Because WSL uses a standard Ubuntu installation, upgrading your packages should look very familiar::

    $ sudo apt-get update
    $ sudo apt-get upgrade

Updating the Ubuntu OS
----------------------

You can aso upgrade to the latest version of Ubuntu with the following command (caution, this will take quite some time)!::

    $ sudo do-release-upgrade -f DistUpgradeViewNonInteractive -d

And, it works, just as expected!
