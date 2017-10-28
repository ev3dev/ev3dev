========================================
Getting Started with LEGO MINDSTORMS EV3
========================================


Hardware Requirements
=====================

You will need *all* of the following:

* `LEGO MINDSTORMS EV3 <https://mindstorms.lego.com>`_ intelligent brick
* MicroSDHC memory card [#sd-card]_
* Windows, macOS or Linux computer with an Internet connection [#host-computer]_
* SD card reader for your computer

.. [#sd-card] Look for the SDHC logo on the card. Cards larger than 32GB are not
   supported and will likely have data corruption issues. Some users with
   32GB cards have also reported data
   corruption issues.
.. [#host-computer] Administrative privileges are needed for installing software and
   flashing the microSD card.


Communication Requirements
==========================

You will need *one* of the following to establish communication to the EV3:

* The USB cable that comes with the EV3
* A Bluetooth capable computer
* A USB Wi-Fi dongle attached to the EV3 [#wifi-dongle]_

.. [#wifi-dongle] A list of known working Wi-Fi dongles can be found on the
   `wiki <https://github.com/ev3dev/ev3dev/wiki/USB-Wi-Fi-Dongles>`_


Installing Ev3dev
=================

Ev3dev is distributed as a disk image that is flashed to your microSD card.

1. Download and install `Etcher <https://etcher.io/>`_.
2. Download the latest ev3dev image for LEGO MINDSTORMS EV3 from the
   `ev3dev downloads page <http://www.ev3dev.org/downloads>`_.

   .. note:: Follow the link on that page for **ev3dev-stretch** snapshot images.

3. Run Etcher and flash the image to the microSD card. :doc:`Click here <using-etcher>`
   if you need detailed instructions on using Etcher.

4. Put the microSD card in the EV3 and turn it on.

.. tip:: `Create a pull tab <http://botbench.com/blog/2013/10/29/ev3-adding-a-pull-tab-to-your-micro-sd-card/>`_
   to make the microSD card easy to remove.


Establishing a Connection
=========================

**USB**

  Simply connect the USB cable and you are good to go.

**Bluetooth**

  .. todo:: Link to BrickMan docs on how to pair with Bluetooth.

**Wi-Fi**

  .. todo:: Link to BrickMan docs on how to setup Wi-Fi.


Setting Up a Development Environment
====================================

Programming tools are the same no matter which ev3dev device you are using, so
continue :doc:`here </programming/ides>`.
