==================================
Getting Started with FatcatLab EVB
==================================


Hardware Requirements
=====================

You will need *all* of the following:

* `FatcatLab EVB <http://fatcatlab.com/product/evb/>`_
* BeagleBone Black or Green
* MicroSDHC memory card [#]_ [#]_
* Windows, macOS or Linux computer with an Internet connection [#]_
* SD card reader for your computer

.. [#] Look for the SDHC logo on the card. Cards larger than 32GB are not
   supported and will likely have data corruption issues. Some users with
   32GB cards have also reported data
   corruption issues.
.. [#] It is not possible to use the built-in eMMC on the BeagleBone because of
   pin conflicts with the EVB cape.
.. [#] Administrative privileges are needed for installing software and
   flashing the microSD card.


Communication Requirements
==========================

You will need *one* of the following to establish communication to the EVB:

* A USB Wi-Fi dongle attached to the BeagleBone [#]_
* An Ethernet cable

.. [#] A list of known working Wi-Fi dongles can be found on the
   `wiki <https://github.com/ev3dev/ev3dev/wiki/USB-Wi-Fi-Dongles>`_


Installing Ev3dev
=================

Ev3dev is distributed as a disk image that is flashed to your microSD card.

1. Download and install `Etcher <https://etcher.io/>`_.
2. Download the latest ev3dev image for **BeagleBone** from the
   `ev3dev downloads page <http://www.ev3dev.org/downloads>`_.

   .. note:: Follow the link on that page for **ev3dev-stretch** snapshot images.

3. Run Etcher and flash the image to the microSD card. :doc:`Click here </using-etcher>`
   if you need detailed instructions on using Etcher.

4. When the flashing is complete, open the ``EV3DEV_BOOT`` drive of the SD card
   on your computer.

   .. tip:: You may need to remove the microSD card and plug it back in to the computer
      before you see the ``EV3DEV_BOOT`` drive.

5. Open the ``uEnv.txt`` file and follow the instructions. You will need to edit
   a line to enable the EVB cape::

       cape=evb

6. Save the changes to ``uEnv.txt`` and close the text editor.

7. Safely eject the microSD card from your computer.

8. Put the microSD card in the BeagleBone and turn it on.

.. tip:: `Create a pull tab <http://botbench.com/blog/2013/10/29/ev3-adding-a-pull-tab-to-your-micro-sd-card/>`_
   to make the microSD card easy to remove.


Establishing a Connection
=========================

**Wi-Fi**

  .. todo:: Link to BrickMan docs on how to setup Wi-Fi.

**Wired Ethernet**

  Connect an Ethernet cable from your Raspberry Pi to your router or network
  switch.


Setting Up Visual Studio Code
=============================

Visual Studio Code is the officially supported programming environment for ev3dev.
We have developed an extension that is used to interact with the EV3 through
VS Code.

.. todo:: May want a link to detailed instructions on installing VS Code and git.

We have "hello world!" tutorials for several programming languages. Follow one
of the links below for step-by-step instructions:

* `Hello Python! <https://github.com/ev3dev/vscode-hello-python#readme>`_
* `Hello Go(lang)! <https://github.com/ev3dev/vscode-hello-go#readme>`_

.. note:: It is possible to use ev3dev without Visual Studio Code, but it
   is up to you to figure out how to do it.
