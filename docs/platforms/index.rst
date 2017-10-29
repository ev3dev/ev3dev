==================
Hardware Platforms
==================

The following hardware platforms are supported by ev3dev.

.. toctree::
    :maxdepth: 1

    evb
    ev3
    brickpi
    brickpi3
    pistorms
    questcape


This table provides a detailed comparison of all of the supported platforms and their features.

+----------------------+---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
|     Manufacturer                           | LEGO                            | Dexter Industries                                                                       | mindsensors.com                 | FatcatLab                      | Quest Institute    |
+======================+=====================+=================================+=======================================+================+================================+=================================+================================+====================+
| Website                                    | mindstorms.lego.com_            | dexterindustries.com_                                                                   | mindsensors.com_                | fatcatlab.com_                 | questforspace.com_ |
+----------------------+---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
| Model Name                                 | EV3                             | BrickPi                               | BrickPi+       | BrickPi3                       | PiStorms                        | EVB                            | QuestCape          |
+----------------------+---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
| Model Number(s)                            | - 31313 (Retail set)            | - BrickPi v1.7.3 [#brickpi-model]_    | - BrickPi v2.8 | - BrickPi v3.2.1               | - PiStorms                      | - EVB v1.0                     | - QuestCape v1.4   |
|                                            | - 45544 (Education Core set)    |                                       |                |                                | - PiStorms-v2                   |                                |                    |
|                                            | - 45500 (EV3 Intelligent Brick) |                                       |                |                                |                                 |                                |                    |
+----------------------+---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
| Compatible CPU Board                       | N/A                             | - Raspberry Pi Zero/Zero W                                                                                                | - BeagleBone (White)                                |
|                                            |                                 | - Raspberry Pi Model A/A+/B/B+                                                                                            | - BeagleBone Black                                  |
|                                            |                                 | - Raspberry Pi 2 Model B                                                                                                  | - BeagleBone Green [#bone_green-grove]_             |
|                                            |                                 | - Raspberry Pi 3 Model B                                                                                                  |   [#bone_green-wireless]_                           |
+----------------------+---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
| Display              | Resolution          | 178x128 pixels [#ev3-display]_  | N/A [#rpi-display]_ [#brickpi-display]_                | N/A [#rpi-display]_            | 320x240 pixels                  | 220x176 pixels                 | 220x176 pixels     |
+                      +---------------------+---------------------------------+                                                        +                                +---------------------------------+--------------------------------+--------------------+
|                      | Color Depth         | 1 bpp [#ev3-grayscale]_         |                                                        |                                | 16 bpp                          | 16 bpp                         | 16 bpp             |
+                      +---------------------+---------------------------------+                                                        +                                +---------------------------------+--------------------------------+--------------------+
|                      | Backlight           | No                              |                                                        |                                | Yes, always on                  | Yes, always on                 | Yes, adjustable    |
+                      +---------------------+---------------------------------+                                                        +                                +---------------------------------+--------------------------------+--------------------+
|                      | Touchscreen         | No                              |                                                        |                                | Yes                             | No                             | No                 |
+----------------------+---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
| Buttons              | Count               | 6                               | 0                                                      | 0                              | 1                               | 6 [#evb-buttons]_              | 6 [#evb-buttons]_  |
+                      +---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
|                      | Center              | Yes                             | No                                                     | No                             | Yes                             | Yes                            | Yes                |
+                      +---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
|                      | Up                  | Yes                             | No                                                     | No                             | No                              | Yes                            | Yes                |
+                      +---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
|                      | Down                | Yes                             | No                                                     | No                             | No                              | Yes                            | Yes                |
+                      +---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
|                      | Left                | Yes                             | No                                                     | No                             | No                              | Yes                            | Yes                |
+                      +---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
|                      | Right               | Yes                             | No                                                     | No                             | No                              | Yes                            | Yes                |
+                      +---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
|                      | Back                | Yes                             | No                                                     | No                             | No                              | Yes                            | Yes                |
+----------------------+---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
| LEDs                                       | 2 - Red/Green                   | 2 - Blue                                               | 1 - Yellow (Amber)             | 2 [#pistorms-leds]_ -           | None                           | None               |
|                                            |                                 |                                                        |                                | Red/Green/Blue                  |                                |                    |
+----------------------+---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
| Speaker                                    | Yes                             | No [#rpi-speaker]_                                     | No [#rpi-speaker]_             | No [#rpi-speaker]_              | Yes                            | No                 |
+----------------------+---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
| Input Ports          | Count               | 4                               | 4 + 1 I2C only                        | 4              | 4 + 1 Grove I2C                | 4                               | 4                              | 4                  |
+                      +---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
|                      | Automatic Detection | Yes                             | No                                                     | No                             | No                              | Yes [#evb_sensor-autodetect]_  | Yes                |
+                      +---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
|                      | EV3 Sensors         | Yes                             | Yes [#brickpi_ev3-sensors]_                            | Yes [#brickpi3_ev3-sensors]_   | Yes [#pistorms_ev3-sensors]_    | Yes                            | Yes                |
+                      +---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
|                      | NXT Sensors         | Yes                             | Yes [#brickpi_nxt-sensors]_                            | Yes                            | Yes [#pistorms_i2c-sensors]_    | Yes                            | Yes                |
+----------------------+---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
| Output Ports         | Count               | 4                               | 4                                                      | 4                              | 4                               | 4                              | 4                  |
+                      +---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
|                      | Automatic Detection | Yes                             | No                                                     | No                             | No                              | Yes                            | Yes                |
+----------------------+---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
| Battery Indication   | Voltage             | Yes                             | No                                    | Yes            | Yes                            | Yes                             | Yes                            | No                 |
+                      +---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
|                      | Current             | Yes                             | No                                    | No             | No                             | No                              | Yes                            | No                 |
+----------------------+---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
| Bluetooth [#bluetooth]_                    | 2.1 + EDR [#ev3-bluetooth]_     | N/A [#rpi-bluetooth]_                                  | N/A [#rpi-bluetooth]_          | N/A [#rpi-bluetooth]_           | N/A                            | N/A                |
+----------------------+---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+
| Wi-Fi [#wifi]_                             | N/A                             | N/A [#rpi-wifi]_                                       | N/A [#rpi-wifi]_               | N/A [#rpi-wifi]_                | N/A                            | N/A                |
+----------------------+---------------------+---------------------------------+---------------------------------------+----------------+--------------------------------+---------------------------------+--------------------------------+--------------------+

.. _mindstorms.lego.com: https://lego.com/mindstorms
.. _dexterindustries.com: https://dexterindustries.com
.. _mindsensors.com: https://mindsensors.com
.. _fatcatlab.com: http://fatcatlab.com
.. _questforspace.com: http://questforspace.com

.. [#brickpi-model] The version number is not actually printed on the BrickPi circuit board.
.. [#bone_green-grove] The Grove sensor ports are not usable with EVB or QuestCape because of shared I/O pins.
.. [#bone_green-wireless] BeagleBone Green Wireless is not supported because of I/O pin conflicts.
.. [#ev3-display] It is possible to replace the display in the EV3. `Video <https://www.youtube.com/watch?v=gPNJC5Uz9HY>`_.
   The color screen is 160x128 pixels, 16 bpp, with adjustable backlight.
.. [#ev3-grayscale] The EV3 display is capable of 2bpp grayscale. We're working on it.
.. [#rpi-display] It is possible to attach an HDMI (or NTSC) display to the Raspberry Pi.
.. [#brickpi-display] It is possible to stack a display on top of BrickPi. `Blog <https://lechnology.com/2016/05/adding-a-display-to-brickpi/>`_.
.. [#evb-buttons] EVB and QuestCape cannot detect simultaneous button presses.
.. [#pistorms-leds] Some hardware revisions of the PiStorms only have 1 physical LED. However, 2 LEDs will still appear in sysfs.
.. [#rpi-speaker] The headphone jack on Raspberry Pi can be used for sound. Sound is not enabled by default.
.. [#evb_sensor-autodetect] The EVB cannot automatically detect some NXT sensors. NXT sensors can still be used, but the input port must be manually configured for them.
.. [#brickpi_ev3-sensors] BrickPi(+) only supports the LEGO EV3 sensors (Color, Infrared, Ultrasonic, Gyro, Touch). 3rd party EV3 sensors will not work.
   `The UART sensor implementation is buggy in the BrickPi(+) firmware <https://github.com/DexterInd/BrickPi/issues/24>`_.
.. [#brickpi3_ev3-sensors] BrickPi3 only supports the LEGO EV3 sensors (Color, Infrared, Ultrasonic, Gyro, Touch). 3rd party EV3 sensors will not work.
.. [#pistorms_ev3-sensors] PiStorms only supports the LEGO EV3 sensors (Color, Infrared, Ultrasonic, Gyro, Touch). 3rd party EV3 sensors will not work.
.. [#brickpi_nxt-sensors] BrickPi(+) has limited I2C sensor support. Most sensors do work, but there may be some limitations.
.. [#pistorms_i2c-sensors] PiStorms shares a single I2C communication bus with all four input ports, so each sensor must have a unique I2C address.
.. [#bluetooth] Bluetooth (include Bluetooth Low Energy) support can be added to any device via a USB Bluetooth dongle.
.. [#ev3-bluetooth] Newer models of the EV3 technically have a Bluetooth 4.0 chip. However, the new chip does **not** have Bluetooth Low Energy (LE) capabilities.
.. [#rpi-bluetooth] Raspberry Pi 3 Model B and Raspberry Pi Zero W have built-in Bluetooth + LE (Low Energy).
.. [#wifi] Wi-Fi support can be added to any device via a USB Wi-Fi dongle.
.. [#rpi-wifi] Raspberry Pi 3 Model B and Raspberry Pi Zero W have built-in Wi-Fi.
