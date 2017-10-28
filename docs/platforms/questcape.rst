=========================
Quest Institute QuestCape
=========================

QuestCape is a LEGO MINDSTORMS compatible daughterboard for `BeagleBone
<http://beagleboard.org/>`_ produced by `The Quest Institute
<http://thequestinstitute.com//>`_ to perform experiments on the International
Space Station as part of their `ISS program <http://www.thequestinstitute.com/ISS/>`_.

.. note:: The design is based on the :doc:`FatcatLab EVB <evb>`, so the hardware
    driver links on this page all point to the EVB docs.


Setup
=====

Since the QuestCape does not have an EEPROM to electronically identify it, some
manual configuration is required to enable it. This is done by editing the
``uEnv.txt`` file in the boot partition::

    # QuestCape
    cape=quest


Power
=====

QuestCape is powered from the 5V jack on the BeagleBone. The motors are powered
separately via a connector on the QuestCape. There is no battery voltage
indication (it is expected to be powered by a fixed power supply).

Motors can be powered from the 5V jack on the BeagleBone, but it is not recommended.


Sensors and Input Ports
=======================

The QuestCape input ports are basically the same as the input ports on LEGO
MINDSTORMS EV3. There are some caveats though.

* It uses Molex connectors on the circuit board instead of the RJ11-style
  connectors used on the EV3.
* A small number of NXT/I2C sensors require 9V (battery voltage) on input port
  pin 1 (e.g. the LEGO NXT Ultrasonic sensor and the Codatex RFID sensor).
  EVB does not provide this voltage.

More information is available in the `hardware driver documentation`__.

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/evb.html#input-output-ports


Motors and Output Ports
=======================

The output ports on the QuestCape are virtually identical to LEGO MINDSTORMS EV3.
It uses Molex connectors on the circuit board instead of the RJ11-style
connectors used on the EV3.

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/evb.html#input-output-ports


Display
=======

EVB has a 2.2" 220x176 pixel color display (16bpp). The backlight is adjustable.

The display board is separate from the main circuit board and can be detached.


Buttons
=======

QuestCape has a small joystick for directional input (up, down, left, right) and
center (enter) plus a separate button for back (backspace). Pressing more than
one button at a time is not supported.

The joystick/button board is separate from the main circuit board and can be
detached.

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/evb.html#buttons-joystick


Sound
=====

QuestCape does **not** have a speaker.


LEDs
====

QuestCape does **not** have any user controllable LEDs.

There are LEDs for power indication (5V and battery voltage).


Bluetooth
=========

EVB does **not** have Bluetooth capabilities. A USB Bluetooth dongle can be used
if needed.


Wi-Fi
=====

EVB does **not** have Wi-Fi capabilities. A USB Wi-Fi dongle can be used if needed.

More information on USB Wi-Fi dongles is available on the `wiki`__.

.. __: https://github.com/ev3dev/ev3dev/wiki/USB-Wi-Fi-Dongles
