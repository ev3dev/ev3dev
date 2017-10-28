============
Fundamentals
============

The following information applies to all programming languages. These are the
basic things you need to know to create and run programs on ev3dev.


File Permissions
================

Linux (and other Unix-like operating systems) have a special file permission
setting to make a file executable. If this permission is not set, then you
cannot run a file directly. Instead, you will get a "Permission denied" error
when you try to run the file.

In the Brickman file browser, executable files have a ``*`` after the file name.
If this ``*`` is missing, you will not be able to run the file from Brickman.

.. tip:: The ev3dev Visual Studio Code extension automatically takes care of setting
    permissions for you, so you don't need to do anything special in that case and
    you can skip reading this section.

If you are transferring files a different way, then you need to need to know
how to set the executable bit.

Command Line
------------

One way to set file permissions is to use a remote terminal
to get command prompt on your device, then run::

    chmod +x my.file

Of course, replace ``my.file`` with the actual name of your file. This tells
the OS to **ch**\ ange the **mod**\ e of the file by setting the e\ *x*\ ecutable
bit globally for the file. This can be verified by running::

    ls -l my.file

This tells the OS to **l**\ i\ **s**\ t some basic information about this file.
You should see something like this::

    -rwxr-xr-x 1 robot robot 0 Oct 28 19:39 my.file

As you can see, ``x`` is actually listed three times in the file permissions
(``-rwxr-xr-x``). This is because each file has three sets of permissions, one
for the **u**\ ser (i.e. ``robot``), one for the **g**\ roup (also ``robot``)
and one for **o**\ thers (everyone).

In terms of ev3dev, the really important one is the first one, the user.

WinSCP
------

.. todo:: Add screenshots that show how to set file permissions using WinSCP.

Filezilla
---------

.. todo:: Add screenshots that show how to set file permissions using Filezilla.


Scripts
=======

A **script** is a text file that can be run as a program. There are many scripting
languages available on ev3dev, such as Bash, Lua, Python and Perl. There are
a few things you need to watch out for when writing scripts.

Although it is possible to run scripts by invoking the interpreter directly,
such as::

    python3 my_script.py

...we don't usually do this in ev3dev. Instead, we do a few things to make the
file work as a stand-alone executable file.

The Shebang
-----------

In Linux (and other Unix-like operating systems), there is a special syntax used
in the first line of a file to tell the operating system which interpreter to
use to run the file. It looks like this::

    #!/usr/bin/env python3

When you run the script, the operating system runs ``/usr/bin/env python3``, which
finds ``python3`` and then runs ``python3 $0`` where ``$0`` is the filename of
your script.

You can also just write the path to the interpreter directly instead of using
``/usr/bin/env``, like this::

    #!/bin/bash

Without a shebang, Linux will fall back to trying to run file as a shell script.
So, if you forget this in your Python program, you will see strange errors about
commands not found and whatnot.

.. tip:: Using ``/usr/bin/env`` is considered best practice for Python, since it
    is more flexible (e.g. when using ``virtualenv``, the Python interpreter in your
    virtual environment may not be the same as the one at ``/usr/bin/python``).

    Furthermore, according to :pep:`394`, if your script is Python 3.x only, you
    should use ``python3`` in your shebang. If your script is Python 2.x only,
    you should use ``python2``. Using ``python`` with no number after it should
    only be used if your script was designed to run with both 2.x and 3.x.

.. note:: The name **shebang** comes from the characters ``#!``. In computer-speak,
   ``#`` is sometimes refered to as a **sh**\ arp or a **sh**\ ell prompt and ``!``
   is often called **bang**.

Line Endings
------------

Line endings are the hidden characters at the end of each line in a text file.
Windows and Linux use different line endings, which can cause problems. Windows
uses two character, a *carriage return* and a *line feed* (also written *CRLF* or
``\r\n``). Linux only uses a single character, a *line feed* (also written *LF*
or ``\n``).

Most interpreters for scripts don't care about line endings. But, Windows line
endings will break the magic `shebang <The Shebang>`_ line we talked about above.
For example, Linux will try to run ``python3\r`` instead of just ``python3`` and
you will get a "File not found" error.

If your program runs when you type ``python3 my_file.py`` but not when you type
``./my_file.py``, this is probably why it is not working.

So, if you are using Windows, be sure to change the line endings in your text
editor to *Unix* or *CRLF* when writing a script for ev3dev. On Linux and macOS,
*Unix* line endings are the default, so you generally don't have to worry about
this.

Executable Bit
--------------

Linux will not let you run just any file directly. The last step needed to make
the magic `shebang <The Shebang>`_ work is to set the executable bit of the file.
See the `File Permissions`_ section above for details.


Running Programs
================

Although you can just run a program from a terminal directly, like this::

    ./my_script.py

...you generally don't want to do this. Why? Well, if your program crashes, for
example, the motors won't stop and your robot might try to destroy itself.

Instead, start your programs using the `brickrun`_ command. This takes care of
some tricky things in ev3dev/Linux, like console switching, and will clean up
after your program when it exits (or crashes). Just add ``brickrun`` before
your program like this::

    brickrun ./my_script.py

.. note:: Brickman and the Visual Studio Code extension both use ``brickrun``
    behind the scenes too, so using ``brickrun`` from the command line will
    ensure that your program runs the same no matter how your start it.

.. todo:: Add links to Brickman docs and Visual Studio Code extension docs about
    running programs.

.. _brickrun: https://github.com/ev3dev/brickrun/blob/ev3dev-stretch/doc/brickrun.rst



Standard I/O
============

All computer programs have standard input and output streams commonly called
``stdin``, ``stdout`` and ``stderr``. Normally, these read from/write to the
terminal that started the program, but they can also be redirected from/to files
or other programs. When you `run programs using ev3dev tools <Running Programs>`_
these streams are handled in a special way.

stdin
-----

If you run a program in a remote terminal, the usual behavior is for ``stdin``
to read whatever is typed into the remote terminal while the program is running.
However, when programs are run with ``brickrun``, ``stdin`` comes from the active
console on the remote device itself. This means you need to press the built-in
buttons on the device or use a keyboard attached to the device instead of typing
into the remote terminal where the program was launched.

The behavior is the same when the program is started without a remote terminal,
e.g. when the program is started from the Brickman user interface, ``stdin`` will
still come from the device itself.

stdout
------

If you run a program in a remote terminal, the usual behavior is for ``stdout``
to print to the remote terminal while the program is running.
However, when programs are run with ``brickrun``, ``stdout`` prints to the active
console on the remote device itself. In other words, it prints to the screen on
the remote device.

The behavior is the same when the program is started without a remote terminal,
e.g. when the program is started from the Brickman user interface, ``stdin`` will
still print to the screen on the device itself.

stderr
------

If you run a program in a remote terminal, the usual behavior is for ``stderr``
to print to the remote terminal while the program is running (just like ``stdout``).
Likewise, when programs are run from a remote terminal with ``brickrun``,
``stderr`` will still print to the remote terminal instead of on the remote device
(unlike ``stdout``).

When running programs from the Brickman user interface, there is no remote terminal,
so ``stderr`` is saved to a file with the same name as your program plus the file
extension ``.err.log`` added to the end. You can read this file to see any errors
from your program. If nothing was printed to ``stderr``, this file will not be
created.

When using the Visual Studio Code extension, ``stderr`` is printed in the *OUTPUT*
pane of Visual Studio Code.

.. note:: ``stderr`` is a second output stream, like ``stdout`` that is used for
    error messages (at least in well-behaved programs). Most of the time, you
    don't notice the difference between the two because they both print to the
    same place. But, they are designed so that you can redirect one but not the
    other if needed.

.. tip:: You can print debug messages to ``stderr`` to help troubleshoot your program.
