========================
Development Environments
========================

`Visual Studio Code <vscode>`_ + the `ev3dev browser extension <ev3dev-browser>`_
is the officially supported programming environment for ev3dev. There are plenty
of other programming tools out there, so if you want to use them instead, it is
your choice (we won't be able to provide as much help though).

.. _vscode: https://code.visualstudio.com/
.. _ev3dev-browser: https://marketplace.visualstudio.com/items?itemName=dlech.ev3dev-browser


Visual Studio Code
==================

.. todo:: Detailed instructions on installing VS Code and the extension.

We have "hello world!" tutorials for several programming languages. Follow one
of the links below for step-by-step instructions:

* `Hello Python! <https://github.com/ev3dev/vscode-hello-python#readme>`_
* `Hello Go(lang)! <https://github.com/ev3dev/vscode-hello-go#readme>`_


Open Roberta Lab
================

`Open Roberta Lab <https://lab.open-roberta.org/>`_ is a web-based programming
environment that is compatible with ev3dev. Currently, only LEGO MINDSTORMS EV3
is supported (it is an open-source project, so if you want to see other platforms
added, you know what to do...).

.. todo:: A screenshot would be nice here.


On-Device Options
=================

It is possible to write programs directly on ev3dev devices without any external
tools needed. For example, ev3dev ships with two text editors, `nano`_ and `vim`_.

Either use a remote SSH terminal or plug in a keyboard and press :kbd:`Alt`\ +\ :kbd:`Ctrl`\ +\ :kbd:`F6`
to get a terminal on the device, then run ``nano my.file`` to start editing a file.

.. _nano: https://manpages.debian.org/stretch/nano/nano.1.en.html
.. _vim: https://manpages.debian.org/stretch/vim-common/vim.1.en.html
