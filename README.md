The ev3dev meta repo [![Join the chat at https://gitter.im/ev3dev/chat](https://badges.gitter.im/ev3dev/chat.svg)](https://gitter.im/ev3dev/chat?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
====================

Ev3dev is an operating system that runs on the LEGO MINDSTORMS EV3 and other platforms with compatible motor/sensor hardware. Its goal is to allow you to write code which controls your MINDSTORMS robots in any language you want, with whatever frameworks and libraries you like to use.

Ev3dev is based on Debian Linux, so any software that runs on Linux and can be built for ARM should be able to run on ev3dev. 

This repository doesn't actually have any code. It hosts [SD card image downloads](https://github.com/ev3dev/ev3dev/releases) and the project-wide  [issues tracker](https://github.com/ev3dev/ev3dev/issues).

### Looking for documentation and tutorials? Check out our [website](http://www.ev3dev.org).

Our website hosts docs, guides and tutorials to help you get up-and-running with ev3dev as quickly as possible. Check out the [getting started guide](http://www.ev3dev.org/docs/getting-started/) if you're looking for a place to jump in.

### Need support or found a bug? Read through our [support page](http://www.ev3dev.org/support/) to find the best place to ask.

We have a Gitter chat room and an IRC channel as well as our GitHub issues tracker that we use to discuss the ev3dev project and track remaining work. The support page explains how you can utilize these tools most effectively.

### Want to get started writing your own programs? Look through the [list of available libraries](http://www.ev3dev.org/docs/libraries/).

We have many contributors that maintain libraries to make it as easy as possible to interface with ev3dev from your code. There's a [centralized repo](https://github.com/ev3dev/ev3dev-lang) with a "unified" library set as well as an overall [list of available libraries](http://www.ev3dev.org/docs/libraries/). Just pick a language, find the corresponding library, and dive into that library's examples. Or, you can always access the drivers directly if your language isn't already implemented as a pre-made library; there's  information on this style on our [docs landing page](http://www.ev3dev.org/docs/).

### Searching for the code that runs ev3dev? Have a look at all of the other repositories in the [ev3dev GitHub organization](https://github.com/ev3dev).

This repo just hosts the "meta content" that spans our many codebases and subprojecs. The code itself is managed granularly on a per-project level, and each gets its own repo.

**Central code repositories:**
- [ev3dev kernel](https://github.com/ev3dev/ev3-kernel): The foundational Linux-based kernel that runs ev3dev.
- [LEGO device drivers](https://github.com/ev3dev/lego-linux-drivers): Drivers that provide control over LEGO MINDSTORMS devices and related hardware.
- [Brickman](https://github.com/ev3dev/brickman): Graphical brick manager for ev3dev.
- [ev3dev website](https://github.com/ev3dev/ev3dev.github.io): The ev3dev website and documentation.
- [brickstrap](https://github.com/ev3dev/brickstrap): The tool that we use to build ev3dev image files.
- [ev3dev-lang language bindings](https://github.com/ev3dev/ev3dev-lang): A centralized collection of libraries for programming your ev3dev robots.

### Looking for something else? You can find most content from our home page at <http://www.ev3dev.org>.
