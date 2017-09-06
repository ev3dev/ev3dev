==============================================
Getting Started with Dexter Industries BrickPi
==============================================


Hardware Requirements
=====================

You will need *all* of the following:

* `Dexter Industries BrickPi, BrickPi+ or BrickPi3 <https://www.dexterindustries.com/brickpi/>`_
* Raspberry Pi Model B, B+, 2 or 3
* A 12V power source [#]_
* A compatible SD or MicroSD memory card [#]_
* Windows, macOS or Linux computer with an Internet connection [#]_
* SD card reader for your computer

.. [#] The power source can be batteries or an AC/DC adapter. Powering via USB
   on the Raspberry Pi will work, but you will not be able to run any motors.
.. [#] Refer to Raspberry Pi `SD Card FAQ <https://www.raspberrypi.org/help/faqs/#topSdCards>`_
.. [#] Administrative privileges are needed for installing software and
   flashing the microSD card.


Communication Requirements
==========================

Since the BrickPi does not have a display, we will be using the wired
Ethernet connection to begin with. A Wi-Fi connection can be setup later.


Installing Ev3dev
=================

Ev3dev is distributed as a disk image that is flashed to your microSD card.

1. Download and install `Etcher <https://etcher.io/>`_.
2. Download the latest ev3dev image for **Raspberry Pi** from the
   `ev3dev downloads page <http://www.ev3dev.org/downloads>`_.

   .. note:: Follow the link on that page for **ev3dev-stretch** snapshot images.

3. Run Etcher and flash the image to the microSD card. :doc:`Click here </using-etcher>`
   if you need detailed instructions on using Etcher.

4. When the flashing is complete, open the ``EV3DEV_BOOT`` drive of the SD card
   on your computer.

   .. tip:: You may need to remove the SD card and plug it back in to the computer
      before you see the ``EV3DEV_BOOT`` drive.

5. Open the ``config.txt`` file and follow the instructions. There are various
   lines that need to edited depending on which models of BrickPi and Raspberry
   Pi you have, so be sure to read carefully.

6. Save the changes to ``config.txt`` and close the text editor.

7. Safely eject the SD card from your computer.

8. Put the SD card in the Raspberry Pi and turn it on.

   .. tip:: If all goes well, the two blue LEDs on the BrickPi or BrickPi+ should turn on.
      On BrickPi3, the single LED should stop blinking and be on solid.


Establishing a Connection
=========================

**Wired Ethernet**

  Connect an Ethernet cable from your Raspberry Pi to your router or network
  switch.

  .. tip:: The connection should be automatically configured. You can confirm
     this by running ``ping ev3dev.local`` in a terminal window on your computer.


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
