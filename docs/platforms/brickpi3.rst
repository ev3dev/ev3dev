==========================
Dexter Industries BrickPi3
==========================

BrickPi3 is a LEGO MINDSTORMS compatible daughterboard for `Raspberry Pi
<https://www.raspberrypi.org/>`_ produced by `Dexter Industries
<https://www.dexterindustries.com/>`_.


Setup
=====

Since the BrickPi3 does not have an EEPROM to electronically identify it, some
manual configuration is required to enable it. This is done by editing the
``config.txt`` file in the boot partition::

    # uncomment if you are using BrickPi3
    dtoverlay=brickpi3

It is also possible to stack more than one BrickPi3 on one Raspberry Pi. In
order for this to work, the ID for each BrickPi3 needs to be configured in
``config.txt``::

    # uncomment only if you are stacking multiple BrickPi3s
    # replace 0123... with actual id number of each BrickPi3
    dtparam=id1=0123456789ABCDEF0123456789ABCDEF
    dtparam=id2=0123456789ABCDEF0123456789ABCDEF
    #dtparam=id3=0123456789ABCDEF0123456789ABCDEF
    #dtparam=id4=0123456789ABCDEF0123456789ABCDEF

The ID can be found by first connecting each board individually and running
:command:`ev3dev-sysinfo`. Currently, ev3dev only supports stacking up to 4
BrickPi3s (although technically more is possible).

.. tip:: The ID configuration is not needed when using only one BrickPi3.


Power
=====

BrickPi3 is powered from 8 AA batteries (nominally 12V).

It is possible to power the Raspberry Pi + BrickPi3 via USB. However, the
motors will not move because the motor controller chips are connected directly
to the battery voltage.

.. warning:: When powering BrickPi3 from USB, it will shutdown because of low
    battery. See https://github.com/ev3dev/ev3dev/issues/989.

    We are working on a workaround.

More information is available in the `hardware driver documentation`__.

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/brickpi3.html#battery


Sensors and Input Ports
=======================

A major difference compared to LEGO MINDSTORMS EV3 is that the BrickPi3
cannot automatically detect sensors. You must manually configure each input
port to tell it what kind of sensor is attached.

Many LEGO MINDSTORMS sensors will work with BrickPi3. There are some caveats
though.

* A small number of NXT/I2C sensors require 9V (battery voltage) on input port
  pin 1 (e.g. the LEGO NXT Ultrasonic sensor and the Codatex RFID sensor).
  BrickPi3 does not provide this voltage.
* Support for EV3/UART and EV3/Analog sensors is hard coded. As a result, only
  the LEGO brand EV3 sensors will work. 3rd party EV3 sensors, like the FatcatLAB
  sensors will not work. (This could be fixed in the BrickPi3 firmware).

More information is available in the `hardware driver documentation`__.

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/brickpi3.html#input-ports


Motors and Output Ports
=======================

A major difference compared to LEGO MINDSTORMS EV3 is that the BrickPi3
cannot automatically detect motors. By default, each output port is configured
for NXT motors.

Passive braking is not implemented in the BrickPi3 firmware. (This is a
seldom-used feature, most people use active braking).

Some other motor driver features may not be implemented or work the same as the
LEGO MINDSTORMS EV3 motor drivers. Please check GitHub issues and open a new
issue if you have questions.

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/brickpi3.html#output-ports


LEDs
====

BrickPi3 has one LED that can be used for status indication.

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/brickpi3.html#leds

There is an additional LED for power indication. It is not user controllable.

Sound
=====

BrickPi3 does **not** have any sound capabilities. However, the headphone jack
on the Raspberry Pi can be used for sound with an external speaker. The sound
driver is not enabled by default and must be turned on by editing ``config.txt``.


Display
=======

BrickPi3 does **not** have a display. However, it is possible to use the HDMI
(or NTSC) connector on the Raspberry Pi to attach a display.


Buttons
=======

BrickPi3 does **not** have any buttons. You can use a USB or Bluetooth
keyboard if needed. A `USB numeric keypad with backspace`__ is sufficient to
navigate the Brickman user interface.

.. __: https://lmddgtfy.net/?q=usb%20numeric%20keypad%20backspace


Bluetooth
=========

BrickPi3 does **not** have Bluetooth capabilities. The built-in Bluetooth
on Raspberry Pi 3 Model B and Raspberry Pi Zero W can be used. A USB Bluetooth
dongle can be used if needed.


Wi-Fi
=====

BrickPi3 does **not** have Wi-Fi capabilities. The built-in Wi-Fi on Raspberry
Pi 3 Model B and Raspberry Pi Zero W can be used. A USB Wi-Fi dongle can be used
if needed.

More information on USB Wi-Fi dongles is available on the `wiki`__.

.. __: https://github.com/ev3dev/ev3dev/wiki/USB-Wi-Fi-Dongles


Firmware
========

The BrickPi3 firmware can be upgraded in place. Simply run the following command::

    sudo update-brickpi3-fw
