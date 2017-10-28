=============
FatcatLab EVB
=============

EVB is a LEGO MINDSTORMS compatible daughterboard for `BeagleBone
<http://beagleboard.org/>`_ produced by `FatcatLab <http://fatcatlab.com/>`_.


Setup
=====

Since the EVB does not have an EEPROM to electronically identify it, some
manual configuration is required to enable it. This is done by editing the
``uEnv.txt`` file in the boot partition::

    # FatcatLab EVB
    cape=evb


Power
=====

EVB is powered from 6 AA batteries (nominally 9V). It is possible to power
the BeagleBone + EVB via USB or the 5V jack on the BeagleBone. However, the
motors will not move because the motor controller chips are connected directly
to the battery voltage.

.. warning:: When powering EVB from USB, it will shutdown because of low
    battery. See https://github.com/ev3dev/ev3dev/issues/989.

    We are working on a workaround.

More information is available in the `hardware driver documentation`__.

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/evb.html#battery



Sensors and Input Ports
=======================

The EVB input ports are basically the same as the input ports on LEGO MINDSTORMS
EV3. There are some caveats though.

* A small number of NXT/I2C sensors require 9V (battery voltage) on input port
  pin 1 (e.g. the LEGO NXT Ultrasonic sensor and the Codatex RFID sensor).
  EVB does not provide this voltage.
* Due to a missing GPIO on pin 2, some NXT sensors cannot be automatically
  detected. These sensors can still be used by manually configuring the port.

More information is available in the `hardware driver documentation`__.

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/evb.html#input-output-ports


Motors and Output Ports
=======================

The output ports on the EVB are virtually identical to LEGO MINDSTORMS EV3.

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/evb.html#input-output-ports


Display
=======

EVB has a 2.2" 220x176 pixel color display (16bpp). The backlight is always on.


Buttons
=======

EVB has a small joystick for directional input (up, down, left, right) and
center (enter) plus a separate button for back (backspace). Pressing more than
one button at a time is not supported.

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/evb.html#buttons-joystick


Sound
=====

EVB has a built-in speaker. It works just like the speaker on LEGO MINDSTORMS EV3.

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/evb.html#sound


LEDs
====

EVB does **not** have any LEDs.


Bluetooth
=========

EVB does **not** have Bluetooth capabilities. A USB Bluetooth dongle can be used
if needed.


Wi-Fi
=====

EVB does **not** have Wi-Fi capabilities. A USB Wi-Fi dongle can be used if needed.

More information on USB Wi-Fi dongles is available on the `wiki`__.

.. __: https://github.com/ev3dev/ev3dev/wiki/USB-Wi-Fi-Dongles
