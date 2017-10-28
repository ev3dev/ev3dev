==================================
Welcome to ev3dev's documentation!
==================================


Introduction
============

ev3dev is a Debian Linux-based operating system that runs on several LEGO
MINDSTORMS compatible platforms including LEGO MINDSTORMS EV3, Raspberry Pi,
and BeagleBone.


Supported Hardware
==================

* `LEGO MINDSTORMS EV3 <http://mindstorms.lego.com>`_

* `Raspberry Pi <https://raspberrypi.org>`_ with one of the following:

  * `Dexter Industries BrickPi, BrickPi+ or BrickPi3 <https://www.dexterindustries.com/brickpi/>`_

  * `Mindsensors PiStorms-v2 <http://www.mindsensors.com/stem-with-robotics/13-pistorms-v2-base-kit-raspberry-pi-brain-for-lego-robot>`_

* `BeagleBone Black/Green <http://beagleboard.org/bone>`_ with:

  * `FatcatLab's EVB <http://fatcatlab.com/product/evb/>`_

Follow the links below for a side-by-side comparison of supported hardware
devices as well as detailed ev3dev-specific information on each device.

.. toctree::
    :maxdepth: 2

    platforms/index


Versions
========

**ev3dev-jessie** is the current stable version. It only receives important bug
fixes and security updates. It is the recommended version for new users.

**ev3dev-stretch** is the current development version. It is currently in beta,
meaning that it is very usable, but we will continue to add new features and
there may occasionally be breaking changes. It is the recommended version for
more adventurous users.


Where to Start
==============

For **ev3dev-jessie**, `getting started instructions and additional documentation
are on the main ev3dev.org website <http://www.ev3dev.org/docs/getting-started/>`_.

For **ev3dev-stretch**, pick the getting started guide based on your device.

.. toctree::
  :hidden:

  getting-started/index

* :doc:`getting-started/ev3`
* :doc:`getting-started/brickpi`
* :doc:`getting-started/pistorms`
* :doc:`getting-started/evb`


Additional Documentation
========================

General information on programming using ev3dev:

.. toctree::
  :maxdepth: 2

  programming/index

The following are links to documentation for various ev3dev sub-projects:

* `Kernel hardware drivers <http://docs.ev3dev.org/projects/lego-linux-drivers/en/ev3dev-stretch/>`_
