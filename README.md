ev3dev Repositories
===================

1. Introduction
2. Features
3. Repository Descriptions
4. How You Can Help


1. Introduction
---------------

This is part of a group of 4 repositories that make up the `ev3dev` Linux distribution for the LEGO MINDSTORMS EV3. Each of the repositories has the same `README.md` file so you can read this one and not miss anything :-)

The place to go for documentation is the [ev3dev wiki](https://github.com/mindboards/ev3dev/wiki). Please use the [Issues](https://github.com/mindboards/ev3dev/issues) section in the ev3dev repository for day-to-day issues.

The [`ev3dev`](https://github.com/mindboards/ev3dev)  distribution is a full Debian 7 (wheezy) Linux distribution running on the 3.3.x kernel that I have customized for the LEGO MINDSTORMS EV3 controller.

Rather than use custom language bindings that use direct access to mmap'ed memory, this distribution aims to allow as many programming languages as possible to access the EV3 peripherals using simple Linux file access. If your favorite programming language is available as an ARM port, and it can read and write files, you can use it to program the EV3.

Currently the `ev3dev` distribution includes the following languages:

- bash/dash
- awk/gawk
- perl
- Lua
- guile
- ruby
- python

The boot screen you'll be greeted with when you log in is:

````
             _____     _
   _____   _|___ /  __| | _____   __
  / _ \ \ / / |_ \ / _` |/ _ \ \ / /
 |  __/\ V / ___) | (_| |  __/\ V / 
  \___| \_/ |____/ \__,_|\___| \_/  

Debian GNU/Linux 7 on LEGO MINDSTORMS EV3!
````

How neat is that?!!!

2. Features
-----------

Features above and beyond the official LEGO kernel include:

- Support for Atheros, Realtek, and other wifi chipsets so you're not stuck with one specific wifi dongle
- Support for ssh terminal sessions
- Ethernet over USB functionality
- Actual user accounts instead of passwordless root access
- Fully upgradeable and customizable install using standard "apt" tools, running on the brick
- nfs file share capability
- ntp clock updates 
- Access to device drivers through user-space filesystem
- Built in text editors like vim and nano
- Prebuilt support for programming languages like Lua, perl, gawk, Python, guile, Ruby, and more
- Support for all host operating systems including Windows, Mac, Linux, Android, even Blackberry!

Don't want to give up your official LEGO MINDSTORMS EV3 kernel and rootfs? You don't need to!

Just install `ev3dev` on any microSD card (min 1GB suggested, but can you even buy one that small anymore?) and plug it into the microSD slot on the EV3. The uboot loader will look on the card, find the ev3dev kernel and happily boot that instead!

When you want to use the official LEGO tools, just shutdown the EV3, unplug the `ev3dev` microSD card and restart the brick.

This is still an early beta, so it's not as polished as the official LEGO offering, but it's getting better every week as we add support for more of the native EV3 drivers.

3. Repository Descriptions
--------------------------

The ev3dev system is kept in 4 repositories, each with a specific purpose. What's cool about this is that you don't need to have a GitHub account unless you want to help develop the project. 

To get started, just look at the Releases tab and grab the latest and greatest ev3dev.img file. Then check out the [ev3dev wiki](https://github.com/mindboards/ev3dev/wiki) for detailed installation instructions for Linux/OSX/Windows.

[`ev3dev`](https://github.com/mindboards/ev3dev) - Assorted scripts to make building the `ev3dev` system easier. Most of the scripts have been pushed over to either the `ev3dev-rootfs` or `ev3dev-modules` directories. This is really just a dummy repository to hold the licence, README, and wiki pages. However, this *is* the place to download `ev3dev` releases.

[`ev3dev-rootfs`](https://github.com/mindboards/ev3dev-rootfs) - Assorted scripts to build the `ev3dev.img` file that is written to the microSD card. You don't need to download this repository unless you want to build the root file system yourself.

[`ev3dev-kernel`](https://github.com/mindboards/ev3dev-kernel) - The source for the kernel. You don't need to download this unless you are going to actually build the kernel. It's a lot easier to just get the microSD card image and kernel/module updates from the `ev3dev` repository.

[`ev3dev-modules`](https://github.com/mindboards/ev3dev-modules) - The source for the `ev3dev` compatible LEGO MINDSTORMS EV3 drivers. You don't need to download this unless you are going to build the modules, or you want to know a bit more about how the drivers work. The pre-compiled module bundles are in the `ev3dev` repository.

4. How You Can Help
-------------------

Building this custom Linux distribution is a lot of work, even on a Linux host system. Because I strongly dislike doing tedious tasks more than once, and I'm a terrible typist, I decided to script a lot of the mudane tasks like building and customizing the rootfs image, and mounting/formatting/populating the microSD card.

Naturally the scripts run on pretty much any modern Linux system, but they don't work on Windows or Mac systems yet because ... well because even if you have a Mac or Windows machine, developing for the Linux kernel is best done on a Linux machine, and you can always use a VM.

However, I must restate that the goal of this project is to be able to control the EV3 from any platform that can ssh or telnet to a network.

Thanks to a generous donor, I now have a Mac, so all the install instructions can now be created for Linux/Mac/Windows systems on one machine :-)

I've done a lot of the heavy lifting to get the distribution to this point, and I'm happy to take community contributions to the repos. Just send me a pull request and I'll look at your updates.

Cheers, and thanks for looking!

Ralph Hempel
