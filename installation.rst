Installing WSL (Bash on Ubuntu on Windows)
==========================================

This document provides step-by-step instructions for installing WSL on your Windows machine. 

Step 1: Enable Developer Mode
-----------------------------

The first thing you need to do is enable developer mode on your Windows machine. 

Go to **Settings -> Update and Security -> For developers**, and click "Developer mode". 

Step 2: Install WSL
-------------------

Next, you need to install WSL. Go to the Start Menu and search for "turn windows features on or off". 
Select that, then check the "Windows Subsystem for Linux (Beta)" checkbox. 

Hit OK. Restart your computer. 

Step 3: Create a Unix Account
-----------------------------

Next, we need to activate WSL from the command-line. Open up a Command Prompt and run the following command::

    > bash

This will setup your Linux environment on Windows! If you see a blank screen at any point during this process, hit enter, and you'll be prompted to create a new username for your Linux account.

Step 4: Enjoy!
--------------