======================================
Dexter Industries BrickPi and BrickPi+
======================================

BrickPi(+) is a LEGO MINDSTORMS compatible daughterboard for `Raspberry Pi
<https://www.raspberrypi.org/>`_ produced by `Dexter Industries
<https://www.dexterindustries.com/>`_.

BrickPi and BrickPi+ are basically the same from the point of view of ev3dev.
The only notable differences are:

* BrickPi+ can monitor battery voltage, BrickPi cannot.
* BrickPi has a 5th input port for I2C only, BrickPi+ does not.

:doc:`BrickPi3 <brickpi3>`, on the other hand, is significantly different.


Setup
=====

Since the BrickPi(+) does not have an EEPROM to electronically identify it, some
manual configuration is required to enable it. This is done by editing the
``config.txt`` file in the boot partition::

    # uncomment both if you are using BrickPi or BrickPi+
    dtoverlay=brickpi
    init_uart_clock=32000000

BrickPi+ additionally supports monitoring batter voltage, which must be enabled
separately::

    # uncomment only if you are using BrickPi+
    dtparam=brickpi_battery=okay

Furthermore, if you are using a Raspberry Pi 3 Model 3, the built-in Bluetooth
conflicts with the BrickPi(+), so there is more to configure::

    # uncomment to disable Bluetooth on RPi 3
    #dtoverlay=pi3-disable-bt


Power
=====

BrickPi(+) is powered from 8 AA batteries (nominally 12V). Only the BrickPi+ is
able to monitor the battery voltage (see `Setup`_ section above to enable).

It is possible to power the Raspberry Pi + BrickPi(+) via USB. However, the
motors will not move because the motor controller chips are connected directly
to the battery voltage.

.. warning:: When powering BrickPi+ from USB, it will shutdown because of low
    battery. See https://github.com/ev3dev/ev3dev/issues/989.

    As a workaround, don't enable ``dtparam=brickpi_battery=okay``.

More information is available in the `hardware driver documentation`__.

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/brickpi.html#battery


Sensors and Input Ports
=======================

A major difference compared to LEGO MINDSTORMS EV3 is that the BrickPi(+)
cannot automatically detect sensors. You must manually configure each input
port to tell it what kind of sensor is attached.

Many LEGO MINDSTORMS sensors will work with BrickPi(+). There are some caveats
though.

* A small number of NXT/I2C sensors require 9V (battery voltage) on input port
  pin 1 (e.g. the LEGO NXT Ultrasonic sensor and the Codatex RFID sensor).
  BrickPi(+) does not provide this voltage.
* Support for EV3/UART and EV3/Analog sensors is hard coded. As a result, only
  the LEGO brand EV3 sensors will work. 3rd party EV3 sensors, like the FatcatLAB
  sensors will not work. (This could be fixed in the BrickPi firmware).
* The EV3/UART sensor implementation in the BrickPi firmware is `buggy
  <https://github.com/DexterInd/BrickPi/issues/24>`_. Your results may vary.

More information is available in the `hardware driver documentation`__.

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/brickpi.html#input-ports

The BrickPi (not BrickPi+) has a 5th input port that can be used with I2C
sensors. This port is connected to Raspberry Pi I2C pins.

Additional information about using port 5 is available in the `hardware driver
documentation`__.

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/brickpi.html#input-port-5


Motors and Output Ports
=======================

A major difference compared to LEGO MINDSTORMS EV3 is that the BrickPi(+)
cannot automatically detect motors. By default, each output port is configured
for NXT motors.

Passive braking is not implemented in the BrickPi(+) firmware. (This is a
seldom-used feature, most people use active braking).

Some other motor driver features may not be implemented or work the same as the
LEGO MINDSTORMS EV3 motor drivers. Please check GitHub issues and open a new
issue if you have questions.

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/brickpi.html#output-ports


LEDs
====

BrickPi(+) has two LEDs that can be used for status indication.

.. todo:: Hardware driver documentation seems to be missing.


Sound
=====

BrickPi(+) does **not** have any sound capabilities. However, the headphone jack
on the Raspberry Pi can be used for sound with an external speaker. The sound
driver is not enabled by default and must be turned on by editing ``config.txt``.


Display
=======

BrickPi(+) does **not** have a display. However, it is possible to use the HDMI
(or NTSC) connector on the Raspberry Pi to attach a display or to `stack a small
TFT display`__.

.. __: https://lechnology.com/2016/05/adding-a-display-to-brickpi/


Buttons
=======

BrickPi(+) does **not** have any buttons. You can use a USB or Bluetooth
keyboard if needed. A `USB numeric keypad with backspace`__ is sufficient to
navigate the Brickman user interface.

.. __: https://lmddgtfy.net/?q=usb%20numeric%20keypad%20backspace


Bluetooth
=========

BrickPi(+) does **not** have Bluetooth capabilities. The built-in Bluetooth
on Raspberry Pi 3 Model B and Raspberry Pi Zero W can be used, *but at reduced
capacity*. A USB Bluetooth dongle can be used if needed.


Wi-Fi
=====

BrickPi(+) does **not** have Wi-Fi capabilities. The built-in Wi-Fi on Raspberry
Pi 3 Model B and Raspberry Pi Zero W can be used. A USB Wi-Fi dongle can be used
if needed.

More information on USB Wi-Fi dongles is available on the `wiki`__.

.. __: https://github.com/ev3dev/ev3dev/wiki/USB-Wi-Fi-Dongles


Firmware
========

It is possible to upgrade the firmware on the BrickPi(+). However, it requires
additional hardware, such as an Arduino UNO to do the flashing. Also, the
documentation from Dexter Industries seems to have gone missing since they
released the BrickPi 3. There is still some information available at
https://github.com/DexterInd/BrickPi/tree/master/Firmware_BrickPi/.

.. note:: It is not clear in the Dexter Industries documentation, but firmware
    version 2.5 is for BrickPi+ only! It does not work on BrickPi. Likewise,
    older firmware versions are for BrickPi only and do not work on BrickPi+.
