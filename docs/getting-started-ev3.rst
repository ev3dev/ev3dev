========================================
Getting Started with LEGO MINDSTORMS EV3
========================================

.. getting-started-ev3

Hardware Requirements
=====================

You will need *all* of the following:

* `LEGO MINDSTORMS EV3 <https://mindstorms.lego.com>`_ intelligent brick
* MicroSDHC memory card (cards > 32GB will not work, most 32GB cards should work, but
  some may have data corruption issues)
* Windows, macOS or Linux computer capable of running `Visual Studio Code
  <https://code.visualstudio.com/>`_

.. note:: It is possible to use ev3dev without Visual Studio Code, but it
   is up to you to figure out how to do it.


Communication Requirements
==========================

You will need *one* of the following to establish commination to the EV3:

* The USB cable that comes with the EV3
* A Bluetooth capable computer
* A supported USB Wi-Fi dongle attached to the EV3

TODO: make a list of supported Wi-Fi dongles somewhere


Installing Ev3dev
=================

Ev3dev is distributed as a disk image that is flashed to your microSD card.

1. Download and install `Etcher <https://etcher.io/>`_.
2. Download the latest ev3dev image from the `ev3dev downloads page <http://www.ev3dev.org/downloads>`_.

   .. note:: Follow the link on that page for **ev3dev-stretch** snapshot images.

3. Run Etcher and flash the image to the microSD card.

   TODO: Add some screenshots here.

4. Put the microSD card in the EV3 and turn it on.


Establishing a Connection
=========================

**USB**

  Simply connect the USB cable and you are good to go.

  TODO: It's currently not this simple. Some manual configuration is required.

**Bluetooth**

  TODO: Link to BrickMan docs on how to pair with Bluetooth.

**Wi-Fi**

  TODO: Link to BrickMan docs on how to setup Wi-Fi.


Setting Up Visual Studio Code
=============================

Visual Studio Code is the officially supported programming environment for ev3dev.
We have developed an extension that is used to interact with the EV3 through
VS Code.

TODO: May want a link to detailed instructions on installing VS Code and git.

We have "hello world!" tutorials for several programming languages. Follow one
of the links below for step-by-step instructions:

* `Hello Python! <https://github.com/ev3dev/vscode-hello-python#readme>`_
* `Hello Go(lang)! <https://github.com/ev3dev/vscode-hello-go#readme>`_
