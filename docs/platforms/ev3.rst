===================
LEGO MINDSTORMS EV3
===================

EV3 is a programmable LEGO brick produced by `LEGO <http://lego.com/>`_.

.. todo:: Add paragraph about CPU and RAM. Maybe flash memory too.


Power
=====

EV3 is powered from 6 AA batteries (nominally 9V) or a rechargeable LiON battery
pack (nominally 7.4V). The rechargeable LiON battery pack is automatically detected.
Users of NiMH rechargeable batteries should manually configure the power supply
driver to protect against over-discharge that could damage the batteries.

More information is available in the `hardware driver documentation`__.

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/ev3.html#battery


Sensors and Input Ports
=======================

.. todo:: Add documentation about sensor types and automatic detection.

More information is available in the `hardware driver documentation`__.

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/ev3.html#input-ports


Motors and Output Ports
=======================

.. todo:: Add documentation about motor types and automatic detection.

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/ev3.html#output-ports


Display
=======

The EV3 has a 178x128 pixel monochrome display.

.. tip:: The display is also capable of operating in a 2bpp grayscale mode.

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/ev3.html#display


Buttons
=======

The EV3 has 6 buttons. These are mapped to keyboard keys (up, down, left, right,
enter and backspace).

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/ev3.html#buttons


Sound
=====

The EV3 has a built-in speaker for sound playback. A standard Linux sound driver
(ALSA) is provided so that it can be used with most Linux programs that support
sound.

There are two modes of operation. The tone or beep mode, which drives the speaker
with a square wave, can be very loud. The PCM playback mode, on the other hand,
tends to be very quiet.

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/ev3.html#sound


LEDs
====

The EV3 has two red/green LEDs. With both red and green are lit at the same time,
the colors mix and appear to be amber (orange/yellow). Unlike the official LEGO
firmware, the left and right LEDs can be independently controlled in ev3dev.

More information is available in the `hardware driver documentation`__

.. __: http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/ev3.html#leds


Bluetooth
=========

The EV3 has a built-in Bluetooth chip.

.. todo:: Write some more about Blueooth and add some useful links on how to
   use it.


Wi-Fi
=====

EVB does **not** have built-in Wi-Fi capabilities. A USB Wi-Fi dongle can be
used if needed.

More information on USB Wi-Fi dongles is available on the `wiki`__.

.. __: https://github.com/ev3dev/ev3dev/wiki/USB-Wi-Fi-Dongles


Firmware
========

The EV3 firmware resides in the built-in 16MB flash memory. Ev3dev runs entirely
from a microSD card and never touches the firmware. To return to the official
LEGO firmware after using ev3dev, simply power off the EV3 and remove the
microSD card, then turn the EV3 back on.

There has also been some progress on developing a version of ev3dev that runs
from the flash memory instead of from a microSD card. If you are interested in
this, please have a look at https://github.com/ev3dev/ev3dev/issues/416.
