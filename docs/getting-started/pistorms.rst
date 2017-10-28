=========================================
Getting Started with Mindsensors PiStorms
=========================================


Hardware Requirements
=====================

You will need *all* of the following:

* `Mindsensors PiStorms-v2 <http://www.mindsensors.com/stem-with-robotics/13-pistorms-v2-base-kit-raspberry-pi-brain-for-lego-robot>`_
* Raspberry Pi Model B, B+, 2 or 3
* A 9V power source [#power-source]_
* A compatible SD or MicroSD memory card [#sd-card]_
* Windows, macOS or Linux computer with an Internet connection [#host-computer]_
* SD card reader for your computer

.. [#power-source] The power source can be batteries or an AD/DC adapter.
.. [#sd-card] Refer to Raspberry Pi `SD Card FAQ <https://www.raspberrypi.org/help/faqs/#topSdCards>`_
.. [#host-computer] Administrative privileges are needed for installing software and
   flashing the microSD card.


Communication Requirements
==========================

You will need *one* of the following to establish communication to the PiStorms:

* A USB Wi-Fi dongle attached to the Raspberry Pi [#wifi-dongle]_
* The built-in Wi-Fi on Raspberry Pi 3
* An Ethernet cable

.. [#wifi-dongle] A list of known working Wi-Fi dongles can be found on the
   `wiki <https://github.com/ev3dev/ev3dev/wiki/USB-Wi-Fi-Dongles>`_


Installing Ev3dev
=================

Ev3dev is distributed as a disk image that is flashed to your microSD card.

1. Download and install `Etcher <https://etcher.io/>`_.
2. Download the latest ev3dev image for **Raspberry Pi** from the
   `ev3dev downloads page <http://www.ev3dev.org/downloads>`_.

   .. note:: Follow the link on that page for **ev3dev-stretch** snapshot images.

3. Run Etcher and flash the image to the microSD card. :doc:`Click here <using-etcher>`
   if you need detailed instructions on using Etcher.

4. When the flashing is complete, open the ``EV3DEV_BOOT`` drive of the SD card
   on your computer.

   .. tip:: You may need to remove the SD card and plug it back in to the computer
      before you see the ``EV3DEV_BOOT`` drive.

5. Open the ``config.txt`` file and follow the instructions. There is a line
   that needs to be edited to enable PiStorms.

6. Save the changes to ``config.txt`` and close the text editor.

7. Safely eject the SD card from your computer.

8. Put the SD card in the Raspberry Pi and turn it on.


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
