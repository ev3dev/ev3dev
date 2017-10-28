====================
Mindsensors PiStorms
====================

PiStorms is a LEGO MINDSTORMS compatible daughterboard for `Raspberry Pi
<https://www.raspberrypi.org/>`_ produced by `mindsensors.com
<http://www.mindsensors.com/>`_.


Setup
=====

Since the PiStorms does not have an EEPROM to electronically identify it, some
manual configuration is required to enable it. This is done by editing the
``config.txt`` file in the boot partition::
    
    # uncomment if you are using PiStorms
    dtoverlay=pistorms


Power
=====

PiStorms is powered from 6 AA batteries (nominally 9V). Powering via USB on the
Raspberry Pi is not supported.

More information is available in the `hardware driver documentation`__.

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/pistorms.html#battery


Sensors and Input Ports
=======================

A major difference compared to LEGO MINDSTORMS EV3 is that the PiStorms
cannot automatically detect sensors. You must manually configure each input
port to tell it what kind of sensor is attached.

Many LEGO MINDSTORMS sensors will work with PiStorms. There are some caveats
though.

* Support for EV3/UART and EV3/Analog sensors is hard coded. As a result, only
  the LEGO brand EV3 sensors will work. 3rd party EV3 sensors, like the FatcatLAB
  sensors will not work. (This could be fixed in the PiStorms firmware).

More information is available in the `hardware driver documentation`__.

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/pistorms.html#input-ports


Motors and Output Ports
=======================

A major difference compared to LEGO MINDSTORMS EV3 is that the PiStorms
cannot automatically detect motors. By default, each output port is configured
for NXT motors.

Some other motor driver features may not be implemented or work the same as the
LEGO MINDSTORMS EV3 motor drivers. Please check GitHub issues and open a new
issue if you have questions.

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/pistorms.html#output-ports


LEDs
====

PiStorms has two RGB LEDs that can be used for status indication.

.. warning:: Some hardware revisions of the PiStorms only have one LED. Two LEDs
   will still be shown in ev3dev even though one is not physically present.

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/pistorms.html#leds


Display
=======

PiStorms has a 2.4" 320x240 pixel color display (16bpp) with a resistive
touchscreen. The backlight is always on.

.. warning:: Touchscreen support is not yet implemented in the Brickman user
   interface. For the time being, you will need an external keyboard. A `USB
   numeric keypad with backspace`__ is sufficient to navigate the Brickman user
   interface.

.. __: https://lmddgtfy.net/?q=usb%20numeric%20keypad%20backspace


Buttons
=======

PiStorms has a single *GO* button that is mapped as the *Enter* button in ev3dev.


Sound
=====

PiStorms does **not** have any sound capabilities. However, the headphone jack
on the Raspberry Pi can be used for sound with an external speaker. The sound
driver is not enabled by default and must be turned on by editing ``config.txt``.


Bluetooth
=========

PiStorms does **not** have Bluetooth capabilities. The built-in Bluetooth
on Raspberry Pi 3 Model B and Raspberry Pi Zero W can be used. A USB Bluetooth
dongle can be used if needed.


Wi-Fi
=====

PiStorms does **not** have Wi-Fi capabilities. The built-in Wi-Fi on Raspberry
Pi 3 Model B and Raspberry Pi Zero W can be used. A USB Wi-Fi dongle can be used
if needed.

More information on USB Wi-Fi dongles is available on the `wiki`__.

.. __: https://github.com/ev3dev/ev3dev/wiki/USB-Wi-Fi-Dongles


Firmware
========

The PiStorms firmware is upgradeable. Currently, ev3dev does not have a package
to provide this functionality. Please see http://www.mindsensors.com/blog/how-to/how-to-upgrade-pistorms-firmware
for instructions. Be sure to disable PiStorms in ``config.txt`` and reboot first
so that the hardware drivers are not trying to use the PiStorms at the same
time you are upgrading the firmware.

.. tip:: Instead of downloading the zip file to your computer and transferIng
   to your Raspberry Pi, you can download it directly on the Raspberry Pi from
   the command line. For example::

       mkdir fwupgrader
       cd fwupgrader
       wget "http://www.mindsensors.com/index.php?controller=attachment&id_attachment=318" --content-disposition
       unzip fwupgrader.zip
       chmod +x fwupgrader

.. warning:: This information seems to be a bit out of date (it doesn't mention
   PiStorms-V2). Please contact mindsensors.com if you have questions about
   upgrading the firmware.
