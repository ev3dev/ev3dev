==================================
Getting Started with FatcatLab EVB
==================================


Hardware Requirements
=====================

You will need *all* of the following:

* `FatcatLab EVB <http://fatcatlab.com/product/evb/>`_
* BeagleBone Black or Green
* A 9V power source [#power-source]_
* MicroSDHC memory card [#sd-card]_ [#emmc]_
* Windows, macOS or Linux computer with an Internet connection [#host-computer]_
* SD card reader for your computer

.. [#power-source] The power source can be batteries or an AC/DC adapter.
.. [#sd-card] Look for the SDHC logo on the card. Cards larger than 32GB are not
   supported and will likely have data corruption issues. Some users with
   32GB cards have also reported data
   corruption issues.
.. [#emmc] It is not possible to use the built-in eMMC on the BeagleBone because of
   pin conflicts with the EVB cape.
.. [#host-computer] Administrative privileges are needed for installing software and
   flashing the microSD card.


Communication Requirements
==========================

You will need *one* of the following to establish communication to the EVB:

* A USB Wi-Fi dongle attached to the BeagleBone [#wifi-dongle]_
* An Ethernet cable

.. [#wifi-dongle] A list of known working Wi-Fi dongles can be found on the
   `wiki <https://github.com/ev3dev/ev3dev/wiki/USB-Wi-Fi-Dongles>`_


Installing Ev3dev
=================

Ev3dev is distributed as a disk image that is flashed to your microSD card.

1. Download and install `Etcher <https://etcher.io/>`_.
2. Download the latest ev3dev image for **BeagleBone** from the
   `ev3dev downloads page <http://www.ev3dev.org/downloads>`_.

   .. note:: Follow the link on that page for **ev3dev-stretch** snapshot images.

3. Run Etcher and flash the image to the microSD card. :doc:`Click here <using-etcher>`
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


Setting Up a Development Environment
====================================

Programming tools are the same no matter which ev3dev device you are using, so
continue :doc:`here </programming/ides>`.
