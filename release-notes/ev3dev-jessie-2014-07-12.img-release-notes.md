Release notes for ev3dev-jessie-2014-07-12.img
==============================================

Changes from previous version
-----------------------------
The previous version was accidentally deleted from GitHub, so this is just a replacement.
The only difference is updated packages (and node.js was added).

Known issues
------------

* Input port 1 is disabled so that it can be used as a serial terminal for debugging.
  Sensors will not work on input port 1.
* Remote SSH sessions hang on reboot or poweroff.
* `plymouth` is not working during boot/shutdown.
* Empty /etc/sudoers file. The correct file is [here](http://sources.debian.net/src/sudo/1.8.9p5-1/debian/sudoers) and file permissions should be `0440`.

Built using
-----------
* Linux Mint 17 Qiana
* brickstrap 0.2.5
* multistrap 2.2.0ubuntu2
* proot 3.2.2-1ev3dev2
* libguestfs-tools 1:1.24.5-1ev3dev1

Included Packages
-----------------

```
Desired=Unknown/Install/Remove/Purge/Hold
| Status=Not/Inst/Conf-files/Unpacked/halF-conf/Half-inst/trig-aWait/Trig-pend
|/ Err?=(none)/Reinst-required (Status,Err: uppercase=bad)
||/ Name                           Version               Architecture Description
+++-==============================-=====================-============-===============================================================================
ii  acl                            2.2.52-1              armel        Access control list utilities
ii  adduser                        3.113+nmu3            all          add and remove users and groups
ii  alsa-utils                     1.0.27.2-1            armel        Utilities for configuring and using ALSA
ii  apt                            1.0.5                 armel        commandline package manager
ii  augeas-lenses                  1.0.0-1.1             all          Set of lenses needed by libaugeas0 to parse config files
ii  base-files                     7.3ev3dev1            armel        Debian base system miscellaneous files
ii  base-passwd                    3.5.28                armel        Debian base system master password and group files
ii  bash                           4.3-7                 armel        GNU Bourne Again SHell
ii  beep                           1.3-3+b1              armel        advanced pc-speaker beeper
ii  bluez                          4.101-4.1             armel        Bluetooth tools and daemons
ii  bluez-tools                    0.1.38+git662e-3      armel        Set of tools to manage Bluetooth devices for linux
ii  bsdmainutils                   9.0.5                 armel        collection of more utilities from FreeBSD
ii  bsdutils                       1:2.20.1-5.8          armel        Basic utilities from 4.4BSD-Lite
ii  ca-certificates                20140325              all          Common CA certificates
ii  console-setup                  1.102                 all          console font and keymap setup program
ii  console-setup-linux            1.102                 all          Linux specific part of console-setup
ii  conspy                         1.10-1                armel        Remote control of Linux virtual consoles
ii  coreutils                      8.21-1.2              armel        GNU core utilities
ii  cpio                           2.11+dfsg-2           armel        GNU cpio -- a program to manage archives of files
ii  dash                           0.5.7-4               armel        POSIX-compliant shell
ii  dbus                           1.8.6-1               armel        simple interprocess messaging system (daemon and utilities)
ii  dconf-gsettings-backend:armel  0.20.0-2              armel        simple configuration storage system - GSettings back-end
ii  dconf-service                  0.20.0-2              armel        simple configuration storage system - D-Bus service
ii  debconf                        1.5.53                all          Debian configuration management system
ii  debian-archive-keyring         2012.4                all          GnuPG archive keys of the Debian archive
ii  debianutils                    4.4                   armel        Miscellaneous utilities specific to Debian
ii  devio                          1.2-1+b1              armel        correctly read (or write) a region of a block device
ii  diffutils                      1:3.3-1               armel        File comparison utilities
ii  dmsetup                        2:1.02.85-2           armel        Linux Kernel Device Mapper userspace library
ii  dosfstools                     3.0.26-2              armel        utilities for making and checking MS-DOS FAT filesystems
ii  dpkg                           1.17.10               armel        Debian package management system
ii  e2fslibs:armel                 1.42.10-1.1           armel        ext2/ext3/ext4 file system libraries
ii  e2fsprogs                      1.42.10-1.1           armel        ext2/ext3/ext4 file system utilities
ii  espeak                         1.47.11-1ev3dev1      armel        Multi-lingual software speech synthesizer
ii  espeak-data:armel              1.47.11-1ev3dev1      armel        Multi-lingual software speech synthesizer: speech data files
ii  ethtool                        1:3.13-1              armel        display or change Ethernet device settings
ii  ev3dev-archive-keyring         0                     all          GnuPG archive keys of the ev3dev archive
ii  ev3dev-base                    5                     armel        Meta package that installs all of the required ev3dev packages.
ii  ev3dev-bluetooth               5                     armel        Firmware and scripts for EV3 bluetooth.
ii  ev3dev-console                 5                     armel        Console related configuration files and console fonts.
ii  ev3dev-flash-kernel            5                     armel        Database entry and boot script for flash-kernel.
ii  ev3dev-i2c                     5                     armel        Udev rules for I2C devices.
ii  ev3dev-leds                    5                     armel        Initialization scripts for EV3 LEDs.
ii  ev3dev-ports                   5                     armel        Scripts related to the EV3 input and output ports
ii  ev3dev-uart                    5                     armel        Firmware and scripts for EV3 input port UARTs.
ii  fbcat                          0.3-1ev3dev1          armel        framebuffer grabber
ii  findutils                      4.4.2-9               armel        utilities for finding files--find, xargs
ii  firmware-atheros               0.43                  all          Binary firmware for Atheros wireless cards
ii  firmware-realtek               0.43                  all          Binary firmware for Realtek wired and wireless network adapters
ii  flash-kernel                   3.22ev3dev1           armel        utility to make certain embedded devices bootable
ii  fontconfig                     2.11.0-5              armel        generic font configuration library - support binaries
ii  fontconfig-config              2.11.0-5              all          generic font configuration library - configuration
ii  fonts-dejavu-core              2.34-1                all          Vera font family derivate with additional characters
ii  gawk                           1:4.1.1+dfsg-1        armel        GNU awk, a pattern scanning and processing language
ii  gcc-4.7-base:armel             4.7.4-1               armel        GCC, the GNU Compiler Collection (base package)
ii  gcc-4.8-base:armel             4.8.3-4               armel        GCC, the GNU Compiler Collection (base package)
ii  gcc-4.9-base:armel             4.9.0-7               armel        GCC, the GNU Compiler Collection (base package)
ii  gir1.2-glib-2.0                1.40.0-2              armel        Introspection data for GLib, GObject, Gio and GModule
ii  glib-networking:armel          2.40.1-2              armel        network-related giomodules for GLib
ii  glib-networking-common         2.40.1-2              all          network-related giomodules for GLib - data files
ii  glib-networking-services       2.40.1-2              armel        network-related giomodules for GLib - D-Bus services
ii  gnupg                          1.4.16-1.2            armel        GNU privacy guard - a free PGP replacement
ii  golang-go                      2:1.3-3               armel        Go programming language compiler
ii  golang-go-linux-arm            2:1.3-3               armel        Go standard library compiled for linux_arm
ii  golang-src                     2:1.3-3               armel        Go programming language compiler - source files
ii  gpgv                           1.4.16-1.2            armel        GNU privacy guard - signature verification tool
ii  grep                           2.18-2                armel        GNU grep, egrep and fgrep
ii  gsettings-desktop-schemas      3.8.2-2               all          GSettings deskop-wide schemas
ii  guile-1.8                      1.8.8+1-9             armel        GNU extension language and Scheme interpreter
ii  guile-1.8-libs                 1.8.8+1-9             armel        Core Guile libraries
ii  gyp                            0.1~svn1729-3         all          Cross-platform build script generator
ii  gzip                           1.6-3                 armel        GNU compression utilities
ii  hostname                       3.15                  armel        utility to set/show the host name or domain name
ii  ifupdown                       0.7.48.1              armel        high level tools to configure network interfaces
ii  init-system-helpers            1.19                  all          helper tools for all init systems
ii  initramfs-tools                0.115                 all          generic modular initramfs generator
ii  initscripts                    2.88dsf-53.2          armel        scripts for initializing and shutting down the system
ii  insserv                        1.14.0-5              armel        boot sequence organizer using LSB init.d script dependency information
ii  iproute                        1:3.15.0-2            all          transitional dummy package for iproute2
ii  iproute2                       3.15.0-2              armel        networking and traffic control tools
ii  iputils-ping                   3:20121221-5+b1       armel        Tools to test the reachability of network hosts
ii  isc-dhcp-client                4.2.4-7               armel        ISC DHCP client
ii  isc-dhcp-common                4.2.4-7               armel        common files used by all the isc-dhcp* packages
ii  kbd                            1.15.5-1              armel        Linux console font and keytable utilities
ii  keyboard-configuration         1.102                 all          system-wide keyboard preferences
ii  klibc-utils                    2.0.3-1               armel        small utilities built with klibc for early boot
ii  kmod                           16-2                  armel        tools for managing Linux kernel modules
ii  less                           458-2                 armel        pager program similar to more
ii  libacl1:armel                  2.2.52-1              armel        Access control list shared library
ii  libapt-pkg4.12:armel           1.0.5                 armel        package management runtime library
ii  libarmadillo4                  1:4.300.8+dfsg-1      armel        streamlined C++ linear algebra library
ii  libarpack2                     3.1.5-3               armel        Fortran77 subroutines to solve large scale eigenvalue problems
ii  libasound2:armel               1.0.27.2-4            armel        shared library for ALSA applications
ii  libasound2-data                1.0.27.2-4            all          Configuration files and profiles for ALSA drivers
ii  libaspell15                    0.60.7~20110707-1     armel        GNU Aspell spell-checker runtime library
ii  libattr1:armel                 1:2.4.47-1            armel        Extended attribute shared library
ii  libaudit-common                1:2.3.7-1             all          Dynamic library for security auditing - common files
ii  libaudit1:armel                1:2.3.7-1             armel        Dynamic library for security auditing
ii  libaugeas-ruby1.9.1            0.5.0-2               all          Transitional package for ruby-augeas
ii  libaugeas0                     1.0.0-1.1             armel        Augeas configuration editing library and API
ii  libblas3                       1.2.20110419-7        armel        Basic Linear Algebra Reference implementations, shared library
ii  libblkid1:armel                2.20.1-5.8            armel        block device id library
ii  libbsd0:armel                  0.6.0-2               armel        utility functions from BSD systems - shared library
ii  libbz2-1.0:armel               1.0.6-5               armel        high-quality block-sorting file compressor library - runtime
ii  libc-ares-dev:armel            1.10.0-2              armel        asynchronous name resolver - development files
ii  libc-ares2:armel               1.10.0-2              armel        asynchronous name resolver
ii  libc-bin                       2.19-5                armel        GNU C Library: Binaries
ii  libc-dev-bin                   2.19-5                armel        GNU C Library: Development binaries
ii  libc6:armel                    2.19-5                armel        GNU C Library: Shared libraries
ii  libc6-dev:armel                2.19-5                armel        GNU C Library: Development Libraries and Header Files
ii  libcairo2:armel                1.12.16-2             armel        The Cairo 2D vector graphics library
ii  libcap-ng0:armel               0.7.3-1.1             armel        An alternate POSIX capabilities library
ii  libcap2:armel                  1:2.22-1.2            armel        support for getting/setting POSIX.1e capabilities
ii  libcap2-bin                    1:2.22-1.2            armel        basic utility programs for using capabilities
ii  libcomerr2:armel               1.42.10-1.1           armel        common error description library
ii  libcroco3:armel                0.6.8-2               armel        Cascading Style Sheet (CSS) parsing and manipulation toolkit
ii  libcryptsetup4:armel           2:1.6.4-4             armel        disk encryption support - shared library
ii  libcurl3-gnutls:armel          7.37.0-1+b1           armel        easy-to-use client-side URL transfer library (GnuTLS flavour)
ii  libdap11:armel                 3.12.0-1              armel        Open-source Project for a Network Data Access Protocol library
ii  libdapclient3:armel            3.12.0-1              armel        Client library for the Network Data Access Protocol
ii  libdapserver7:armel            3.12.0-1              armel        Server library for the Network Data Access Protocol
ii  libdatrie1:armel               0.2.8-1               armel        Double-array trie library
ii  libdb5.3:armel                 5.3.28-5              armel        Berkeley v5.3 Database Libraries [runtime]
ii  libdbd-mysql-ruby1.9.1         0.4.4+gem2deb-1       all          Transitional package for ruby-dbd-mysql
ii  libdbd-pg-ruby1.9.1            0.3.9+gem2deb-1       all          Transitional package for ruby-dbd-pg
ii  libdbi1:armel                  0.9.0-2               armel        DB Independent Abstraction Layer for C -- shared library
ii  libdbus-1-3:armel              1.8.6-1               armel        simple interprocess messaging system (library)
ii  libdbus-glib-1-2:armel         0.102-1               armel        simple interprocess messaging system (GLib-based shared library)
ii  libdconf1:armel                0.20.0-2              armel        simple configuration storage system - runtime library
ii  libdevmapper-event1.02.1:armel 2:1.02.85-2           armel        Linux Kernel Device Mapper event support library
ii  libdevmapper1.02.1:armel       2:1.02.85-2           armel        Linux Kernel Device Mapper userspace library
ii  libdpkg-ruby1.9.1              0.3.8                 all          Transitional package for ruby-debian
ii  libdrm2:armel                  2.4.54-1              armel        Userspace interface to kernel DRM services -- runtime
ii  libedit2:armel                 3.1-20140620-1        armel        BSD editline and history libraries
ii  libee0                         0.4.1-1.1             armel        Event expression library inspired by CEE
ii  libegl1-mesa:armel             10.2.2-1              armel        free implementation of the EGL API -- runtime
ii  libepsilon1:armel              0.9.2-2               armel        Library for wavelet image compression
ii  libespeak1:armel               1.47.11-1ev3dev1      armel        Multi-lingual software speech synthesizer: shared library
ii  libestr0                       0.1.9-1               armel        Helper functions for handling strings (lib)
ii  libestraier8                   1.4.13-13             armel        full-text search system Libraries [runtime]
ii  libevent-2.0-5:armel           2.0.21-stable-1       armel        Asynchronous event notification library
ii  libexpat1:armel                2.1.0-6               armel        XML parsing C library - runtime library
ii  libextlib-ruby1.9.1            0.9.15-3              all          Transitional package for ruby-extlib
ii  libfcgi-ruby1.9.1              0.9.2.1-1             all          Transitional package for ruby-fcgi / libfcgi-ruby1.9.1
ii  libfcgi0ldbl                   2.4.0-8.2             armel        Shared library of FastCGI
ii  libffi6:armel                  3.1-2                 armel        Foreign Function Interface library runtime
ii  libflexmock-ruby1.9.1          0.9.0-1               all          Transitional package for ruby-flexmock
ii  libfontconfig1:armel           2.11.0-5              armel        generic font configuration library - runtime
ii  libfreetype6:armel             2.5.2-1               armel        FreeType 2 font engine, shared library files
ii  libfreexl1:armel               1.0.0g-1              armel        library for direct reading of Microsoft Excel spreadsheets
ii  libfribidi0:armel              0.19.6-1              armel        Free Implementation of the Unicode BiDi algorithm
ii  libgbm1:armel                  10.2.2-1              armel        generic buffer management API -- runtime
ii  libgcc1:armel                  1:4.9.0-7             armel        GCC support library
ii  libgcrypt11:armel              1.5.3-4               armel        LGPL Crypto library - runtime library
ii  libgcrypt20:armel              1.6.1-2               armel        LGPL Crypto library - runtime library
ii  libgctp0d:armel                2.0-1                 armel        General Cartographic Transformation Package Library
ii  libgd3:armel                   2.1.0-3+b1            armel        GD Graphics Library
ii  libgdal1h                      1.10.1+dfsg-5+b3      armel        Geospatial Data Abstraction Library
ii  libgdbm3:armel                 1.8.3-12+b1           armel        GNU dbm database routines (runtime version)
ii  libgdk-pixbuf2.0-0:armel       2.30.7-1              armel        GDK Pixbuf library
ii  libgdk-pixbuf2.0-common        2.30.7-1              all          GDK Pixbuf library - data files
ii  libgeos-3.4.2                  3.4.2-5               armel        Geometry engine for Geographic Information Systems - C++ Library
ii  libgeos-c1                     3.4.2-5               armel        Geometry engine for Geographic Information Systems - C Library
ii  libgfortran3:armel             4.9.0-7               armel        Runtime library for GNU Fortran applications
ii  libgif4:armel                  4.1.6-11              armel        library for GIF images (library)
ii  libgirepository-1.0-1          1.40.0-2              armel        Library for handling GObject introspection data (runtime library)
ii  libgl1-mesa-glx:armel          10.2.2-1              armel        free implementation of the OpenGL API -- GLX runtime
ii  libglapi-mesa:armel            10.2.2-1              armel        free implementation of the GL API -- shared library
ii  libglib2.0-0:armel             2.40.0-3              armel        GLib library of C routines
ii  libgmp10:armel                 2:6.0.0+dfsg-4        armel        Multiprecision arithmetic library
ii  libgnutls-deb0-28:armel        3.2.15-2              armel        GNU TLS library - main runtime library
ii  libgnutls-openssl27:armel      3.2.15-2              armel        GNU TLS library - OpenSSL wrapper
ii  libgnutls26:armel              2.12.23-17            armel        GNU TLS library - runtime library
ii  libgpg-error0:armel            1.13-0.1              armel        library for common error values and messages in GnuPG components
ii  libgpm2:armel                  1.20.4-6.1            armel        General Purpose Mouse - shared library
ii  libgraphite2-3:armel           1.2.4-3               armel        Font rendering engine for Complex Scripts -- library
ii  libgssapi-krb5-2:armel         1.12.1+dfsg-3         armel        MIT Kerberos runtime libraries - krb5 GSS-API Mechanism
ii  libgssglue1:armel              0.4-2                 armel        mechanism-switch gssapi library
ii  libgudev-1.0-0:armel           204-14                armel        GObject-based wrapper library for libudev
ii  libharfbuzz0b:armel            0.9.29-1              armel        OpenType text shaping engine (shared library)
ii  libhdf4-0-alt                  4.2r4-13              armel        Hierarchical Data Format 4 library -- library package
ii  libhdf5-7:armel                1.8.12+docs-1.1+b1    armel        Hierarchical Data Format 5 (HDF5) - runtime files - serial version
ii  libhdfeos5-ruby1.9.1           1.2-1                 all          Transitional package for ruby-hdfeos5
ii  libhdfeos5-ruby1.9.1-dbg       1.2-1                 all          Transitional package for ruby-hdfeos5-dbg
ii  libhe5-hdfeos0:armel           5.1.15.dfsg.1-1       armel        Earth Observation System extensions to HDF5
ii  libhogweed2:armel              2.7.1-2+b1            armel        low level cryptographic library (public-key cryptos)
ii  libhtree-ruby1.9.1             0.8+dfsg-2            all          Transitional package from libhtree-ruby1.9.1 to ruby-htree
ii  libicu52:armel                 52.1-4                armel        International Components for Unicode
ii  libidn11:armel                 1.28-2                armel        GNU Libidn library, implementation of IETF IDN specifications
ii  libjasper1:armel               1.900.1-debian1-2     armel        JasPer JPEG-2000 runtime library
ii  libjbig0:armel                 2.0-2.1               armel        JBIGkit libraries
ii  libjpeg8:armel                 8d1-1                 armel        Independent JPEG Group's JPEG runtime library
ii  libjs-jquery                   1.7.2+dfsg-3          all          JavaScript library for dynamic web applications
ii  libjs-node-uuid                1.4.0-1               all          simple, fast generation of RFC4122 UUIDs - JavaScript library
ii  libjson-c2:armel               0.11-4                armel        JSON manipulation library - shared library
ii  libk5crypto3:armel             1.12.1+dfsg-3         armel        MIT Kerberos runtime libraries - Crypto Library
ii  libkeyutils1:armel             1.5.9-4               armel        Linux Key Management Utilities (library)
ii  libklibc                       2.0.3-1               armel        minimal libc subset for use with initramfs
ii  libkml0:armel                  1.3.0~r864+dfsg-1     armel        Library to manipulate KML 2.2 OGC standard files
ii  libkmod2:armel                 16-2                  armel        libkmod shared library
ii  libkrb5-3:armel                1.12.1+dfsg-3         armel        MIT Kerberos runtime libraries
ii  libkrb5support0:armel          1.12.1+dfsg-3         armel        MIT Kerberos runtime libraries - Support library
ii  liblapack3                     3.5.0-2               armel        Library of linear algebra routines 3 - shared version
ii  liblcms2-2:armel               2.6-3                 armel        Little CMS 2 color management library
ii  libldap-2.4-2:armel            2.4.39-1              armel        OpenLDAP libraries
ii  liblocale-gettext-perl         1.05-8                armel        module using libc functions for internationalization in Perl
ii  liblogging-stdlog0:armel       1.0.4-1               armel        easy to use and lightweight logging library
ii  liblognorm0                    0.3.7-1               armel        Log normalizing library
ii  libltdl7:armel                 2.4.2-1.7             armel        A system independent dlopen wrapper for GNU libtool
ii  liblzma5:armel                 5.1.1alpha+20120614-2 armel        XZ-format compression library
ii  libmapscript-ruby1.9.1         6.4.1-4+b1            armel        Transitional package from libmapscript-ruby1.9.1 to ruby-mapscript
ii  libmapserver1                  6.4.1-4+b1            armel        Shared library for MapServer
ii  libmm-glib0:armel              1.2.0-1               armel        D-Bus service for managing modems - shared libraries
ii  libmount1                      2.20.1-5.8            armel        block device id library
ii  libmpfr4:armel                 3.1.2-1               armel        multiple precision floating-point computation
ii  libmysqlclient18:armel         5.5.37-1              armel        MySQL database client library
ii  libncurses5:armel              5.9+20140118-1        armel        shared libraries for terminal handling
ii  libncursesw5:armel             5.9+20140118-1        armel        shared libraries for terminal handling (wide character support)
ii  libnetcdfc7                    1:4.1.3-7+b1          armel        Interface for scientific data access to large binary data
ii  libnetpbm10                    2:10.0-15+b2          armel        Graphics conversion tools shared libraries
ii  libnettle4:armel               2.7.1-2+b1            armel        low level cryptographic library (symmetric and one-way cryptos)
ii  libnewt0.52:armel              0.52.17-1             armel        Not Erik's Windowing Toolkit - text mode windowing with slang
ii  libnfsidmap2:armel             0.25-5                armel        NFS idmapping library
ii  libnl-3-200:armel              3.2.24-2              armel        library for dealing with netlink sockets
ii  libnl-genl-3-200:armel         3.2.24-2              armel        library for dealing with netlink sockets - generic netlink
ii  libnl-route-3-200:armel        3.2.24-2              armel        library for dealing with netlink sockets - route interface
ii  libnm-glib4:armel              0.9.8.10-4            armel        network management framework (GLib shared library)
ii  libnm-util2:armel              0.9.8.10-4            armel        network management framework (shared library)
ii  libodbc1:armel                 2.3.1-3               armel        ODBC library for Unix
ii  libogdi3.2                     3.2.0~beta2-7.1       armel        Open Geographic Datastore Interface Library -- library
ii  libopenjpeg5:armel             1.5.2-2               armel        JPEG 2000 image compression/decompression library - runtime
ii  libopts25:armel                1:5.18.3-5            armel        automated option processing library based on autogen
ii  libp11-kit0:armel              0.20.2-5              armel        Library for loading and coordinating access to PKCS#11 modules - runtime
ii  libpacket-ruby1.9.1            0.1.15-5              all          Transitional package for ruby-packet
ii  libpam-modules:armel           1.1.8-3               armel        Pluggable Authentication Modules for PAM
ii  libpam-modules-bin             1.1.8-3               armel        Pluggable Authentication Modules for PAM - helper binaries
ii  libpam-runtime                 1.1.8-3               all          Runtime support for the PAM library
ii  libpam-systemd:armel           204-14                armel        system and service manager - PAM module
ii  libpam0g:armel                 1.1.8-3               armel        Pluggable Authentication Modules library
ii  libpango-1.0-0:armel           1.36.3-1              armel        Layout and rendering of internationalized text
ii  libpangocairo-1.0-0:armel      1.36.3-1              armel        Layout and rendering of internationalized text
ii  libpangoft2-1.0-0:armel        1.36.3-1              armel        Layout and rendering of internationalized text
ii  libparted0debian1:armel        2.3-20                armel        disk partition manipulator - shared library
ii  libpcre3:armel                 1:8.31-5              armel        Perl 5 Compatible Regular Expression Library - runtime files
ii  libpcsclite1:armel             1.8.11-3              armel        Middleware to access a smart card using PC/SC (library)
ii  libpixman-1-0:armel            0.32.4-1              armel        pixel-manipulation library for X and cairo
ii  libpng12-0:armel               1.2.50-1              armel        PNG library - runtime
ii  libpolkit-agent-1-0:armel      0.105-6               armel        PolicyKit Authentication Agent API
ii  libpolkit-backend-1-0:armel    0.105-6               armel        PolicyKit backend API
ii  libpolkit-gobject-1-0:armel    0.105-6               armel        PolicyKit Authorization API
ii  libpoppler46:armel             0.26.2-2              armel        PDF rendering library
ii  libpopt0:armel                 1.16-8                armel        lib for parsing cmdline parameters
ii  libpq5:armel                   9.3.4-2               armel        PostgreSQL C client library
ii  libprocps3:armel               1:3.3.9-5             armel        library for accessing process information from /proc
ii  libproj0                       4.8.0-5               armel        Cartographic projection library
ii  libproxy1:armel                0.4.11-4              armel        automatic proxy configuration management library (shared)
ii  libpython-stdlib:armel         2.7.6-2               armel        interactive high-level object-oriented language (default python version)
ii  libpython2.7-minimal:armel     2.7.8-1               armel        Minimal subset of the Python language (version 2.7)
ii  libpython2.7-stdlib:armel      2.7.8-1               armel        Interactive high-level object-oriented language (standard library, version 2.7)
ii  libqdbm14                      1.8.78-4              armel        QDBM Database Libraries without GDBM wrapper[runtime]
ii  librack-ruby1.9.1              1.5.2-1               all          Transitional package for ruby-rack
ii  libramaze-ruby1.9.1            2012.12.08-3          all          Transitional package for ruby-ramaze
ii  libraspell-ruby1.9.1           1.3-1                 all          Transitional package for raspell
ii  libreadline5:armel             5.2+dfsg-2            armel        GNU readline and history libraries, run-time libraries
ii  libreadline6:armel             6.3-6                 armel        GNU readline and history libraries, run-time libraries
ii  librrd-ruby1.9.1               1.4.8-1               all          Transitional package to ruby-rrd
ii  librrd4                        1.4.8-1+b1            armel        time-series data storage and display system (runtime library)
ii  librsvg2-2:armel               2.40.2-1              armel        SAX-based renderer library for SVG files (runtime)
ii  libruby2.1:armel               2.1.2-2               armel        Libraries necessary to run Ruby 2.1
ii  libsamplerate0:armel           0.1.8-7               armel        Audio sample rate conversion library
ii  libsasl2-2:armel               2.1.26.dfsg1-10       armel        Cyrus SASL - authentication abstraction library
ii  libsasl2-modules-db:armel      2.1.26.dfsg1-10       armel        Cyrus SASL - pluggable authentication modules (DB)
ii  libselinux1:armel              2.3-1                 armel        SELinux runtime shared libraries
ii  libsemanage-common             2.3-1                 all          Common files for SELinux policy management libraries
ii  libsemanage1:armel             2.3-1                 armel        SELinux policy management library
ii  libsepol1:armel                2.3-1                 armel        SELinux library for manipulating binary security policies
ii  libsigsegv2:armel              2.10-4                armel        Library for handling page faults in a portable way
ii  libslang2:armel                2.2.4-17              armel        S-Lang programming library - runtime version
ii  libsonic0:armel                0.1.17-1.1            armel        Simple library to speed up or slow down speech
ii  libsoup2.4-1:armel             2.46.0-2              armel        HTTP library implementation in C -- Shared library
ii  libspatialite5:armel           4.1.1-10              armel        Geospatial extension for SQLite - libraries
ii  libsqlite3-0:armel             3.8.5-2               armel        SQLite 3 shared library
ii  libss2:armel                   1.42.10-1.1           armel        command-line interface parsing library
ii  libssh2-1:armel                1.4.3-3               armel        SSH2 client-side library
ii  libssl-dev:armel               1.0.1h-3              armel        Secure Sockets Layer toolkit - development files
ii  libssl1.0.0:armel              1.0.1h-3              armel        Secure Sockets Layer toolkit - shared libraries
ii  libstdc++6:armel               4.9.0-7               armel        GNU Standard C++ Library v3
ii  libstfl-ruby                   0.22-1.1+b2           armel        Ruby bindings for the structured terminal forms language/library
ii  libstfl-ruby1.9.1              0.22-1.1+b2           armel        Ruby 1.9.1 bindings for the structured terminal forms language/library
ii  libsvg-graph-ruby1.9.1         1.0.5-2               all          Transitional package for ruby-svg-graph
ii  libsystemd-daemon0:armel       204-14                armel        systemd utility library
ii  libsystemd-journal0:armel      204-14                armel        systemd journal utility library
ii  libsystemd-login0:armel        204-14                armel        systemd login utility library
ii  libtasn1-6:armel               4.0-2                 armel        Manage ASN.1 structures (runtime)
ii  libtext-charwidth-perl         0.04-7+b2             armel        get display widths of characters on the terminal
ii  libtext-iconv-perl             1.7-5+b1              armel        converts between character sets in Perl
ii  libtext-wrapi18n-perl          0.06-7                all          internationalized substitute of Text::Wrap
ii  libthai-data                   0.1.20-3              all          Data files for Thai language support library
ii  libthai0:armel                 0.1.20-3              armel        Thai language support library
ii  libtiff5:armel                 4.0.3-9               armel        Tag Image File Format (TIFF) library
ii  libtinfo5:armel                5.9+20140118-1        armel        shared low-level terminfo library for terminal handling
ii  libtirpc1:armel                0.2.3-2               armel        transport-independent RPC library
ii  libuconv-ruby1.9.1             0.6.1-1               all          Unicode/EUC-JP translation module for Ruby (transitional package)
ii  libudev1:armel                 204-14                armel        libudev shared library
ii  liburiparser1                  0.7.5-1               armel        URI parsing library compliant with RFC 3986
ii  libusb-0.1-4:armel             2:0.1.12-24           armel        userspace USB programming library
ii  libusb-1.0-0:armel             2:1.0.19-1            armel        userspace USB programming library
ii  libustr-1.0-1:armel            1.0.4-3               armel        Micro string library: shared library
ii  libuuid-perl                   0.05-1                armel        Perl extension for using UUID interfaces as defined in e2fsprogs
ii  libuuid1:armel                 2.20.1-5.8            armel        Universally Unique ID library
ii  libv8-3.14-dev                 3.14.5.8-8            armel        V8 JavaScript engine - development files for 3.14 branch
ii  libv8-3.14.5                   3.14.5.8-8            armel        V8 JavaScript engine - runtime library
ii  libvalidatable-ruby1.9.1       1.6.7-9               all          Transitional package for ruby-validatable
ii  libvpx1:armel                  1.3.0-2               armel        VP8 video codec (shared library)
ii  libwayland-client0:armel       1.5.0-1               armel        wayland compositor infrastructure - client library
ii  libwayland-server0:armel       1.5.0-1               armel        wayland compositor infrastructure - server library
ii  libwebp5:armel                 0.4.0-4.1             armel        Lossy compression of digital photographic images.
ii  libwirble-ruby1.9.1            0.1.3-4               all          Transitional package for ruby-wirble
ii  libwrap0:armel                 7.6.q-25              armel        Wietse Venema's TCP wrappers library
ii  libx11-6:armel                 2:1.6.2-2             armel        X11 client-side library
ii  libx11-data                    2:1.6.2-2             all          X11 client-side library
ii  libx11-xcb1:armel              2:1.6.2-2             armel        Xlib/XCB interface library
ii  libxau6:armel                  1:1.0.8-1             armel        X11 authorisation library
ii  libxcb-dri2-0:armel            1.10-3                armel        X C Binding, dri2 extension
ii  libxcb-dri3-0:armel            1.10-3                armel        X C Binding, dri3 extension
ii  libxcb-glx0:armel              1.10-3                armel        X C Binding, glx extension
ii  libxcb-present0:armel          1.10-3                armel        X C Binding, present extension
ii  libxcb-render0:armel           1.10-3                armel        X C Binding, render extension
ii  libxcb-shape0:armel            1.10-3                armel        X C Binding, shape extension
ii  libxcb-shm0:armel              1.10-3                armel        X C Binding, shm extension
ii  libxcb-sync1:armel             1.10-3                armel        X C Binding, sync extension
ii  libxcb-xfixes0:armel           1.10-3                armel        X C Binding, xfixes extension
ii  libxcb1:armel                  1.10-3                armel        X C Binding
ii  libxdamage1:armel              1:1.1.4-1             armel        X11 damaged region extension library
ii  libxdmcp6:armel                1:1.1.1-1             armel        X11 Display Manager Control Protocol library
ii  libxerces-c3.1:armel           3.1.1-5               armel        validating XML parser library for C++
ii  libxext6:armel                 2:1.3.2-1             armel        X11 miscellaneous extension library
ii  libxfixes3:armel               1:5.0.1-1             armel        X11 miscellaneous 'fixes' extension library
ii  libxml2:armel                  2.9.1+dfsg1-3         armel        GNOME XML library
ii  libxpm4:armel                  1:3.5.10-1            armel        X11 pixmap library
ii  libxrender1:armel              1:0.9.8-1             armel        X Rendering Extension client library
ii  libxshmfence1:armel            1.1-2                 armel        X shared memory fences - shared library
ii  libxslt1.1:armel               1.1.28-2              armel        XSLT 1.0 processing library - runtime library
ii  libxxf86vm1:armel              1:1.1.3-1             armel        X11 XFree86 video mode extension library
ii  libyaml-0-2:armel              0.1.4-3.2             armel        Fast YAML 1.1 parser and emitter library
ii  libzip-ruby1.9.1               1.1.2-1               all          Transitional package for ruby-zip
ii  linux-base                     3.5                   all          Linux image base package
ii  linux-image-3.14.7-1-ev3dev    1                     armel        Linux kernel binary image for version 3.14.7-1-ev3dev
ii  linux-image-ev3dev             4                     armel        Linux kernel for ev3dev (meta-package)
ii  linux-libc-dev:armel           3.14.9-1              armel        Linux support headers for userspace development
ii  locales                        2.19-5                all          GNU C Library: National Language (locale) data [support]
ii  login                          1:4.2-2               armel        system login tools
ii  lsb-base                       4.1+Debian13          all          Linux Standard Base 4.1 init script functionality
ii  lua5.1                         5.1.5-5               armel        Simple, extensible, embeddable programming language
ii  lvm2                           2.02.106-2            armel        Linux Logical Volume Manager
ii  mawk                           1.3.3-17              armel        a pattern scanning and text processing language
ii  mime-support                   3.56                  all          MIME files 'mime.types' & 'mailcap', and support programs
ii  mount                          2.20.1-5.8            armel        Tools for mounting and manipulating filesystems
ii  multiarch-support              2.19-5                armel        Transitional package to ensure multiarch compatibility
ii  mysql-common                   5.5.37-1              all          MySQL database common files, e.g. /etc/mysql/my.cnf
ii  nano                           2.2.6-1.1             armel        small, friendly text editor inspired by Pico
ii  ncurses-base                   5.9+20140118-1        all          basic terminal type definitions
ii  ncurses-bin                    5.9+20140118-1        armel        terminal-related programs and man pages
ii  net-tools                      1.60-26               armel        NET-3 networking toolkit
ii  netbase                        5.2                   all          Basic TCP/IP networking system
ii  netcat-openbsd                 1.105-7               armel        TCP/IP swiss army knife
ii  netpbm                         2:10.0-15+b2          armel        Graphics conversion tools between image formats
ii  network-manager                0.9.8.10-4            armel        network management framework (daemon and userspace tools)
ii  nfs-common                     1:1.2.8-6             armel        NFS support files common to client and server
ii  node-abbrev                    1.0.4-2               all          Like ruby abbrev module, but for Node.js
ii  node-ansi                      0.2.1-1               all          Advanced ANSI formatting tool for Node.js
ii  node-ansi-color-table          1.0.0-1               all          Color and format tables for ansi output - Node.js module
ii  node-archy                     0.0.2-1               all          Pretty-print nested hierarchies module for Node.js
ii  node-async                     0.8.0-1               all          higher-order functions and common patterns for asynchronous Javascript
ii  node-block-stream              0.0.7-1               all          Stream of fixed-size blocks, with zero-padding when necessary
ii  node-combined-stream           0.0.5-1               all          Append streams one after another - module for Node.js
ii  node-cookie-jar                0.3.1-1               all          Cookie handling for HTTP clients - module for Node.js
ii  node-delayed-stream            0.0.5-1               all          Buffer stream events for later handling - module for Node.js
ii  node-forever-agent             0.5.1-1               all          HTTP agent supporting keep-alive requests - module for Node.js
ii  node-form-data                 0.1.0-1               all          Create multipart/form-data streams module for Node.js
ii  node-fstream                   0.1.24-1              all          Advanced filesystem streaming tools for Node.js
ii  node-fstream-ignore            0.0.6-2               all          Directory reader configurable by .ignore module for Node.js
ii  node-github-url-from-git       1.1.1-1               all          Convert github git or gist url to an http url - Node.js module
ii  node-glob                      3.2.6-1               all          glob functionality for Node.js
ii  node-graceful-fs               2.0.0-2               all          drop-in replacement improving the Node.js fs module
ii  node-gyp                       0.12.2+ds-1           all          Native addon build tool for Node.js
ii  node-inherits                  2.0.0-1               all          Exposes inherits function from Node.js environment
ii  node-ini                       1.1.0-1               all          ini format parser and serializer for Node.js
ii  node-json-stringify-safe       5.0.0-1               all          JSON.stringify with circular references module for Node.js
ii  node-lockfile                  0.4.1-1               all          Asynchronous file lock module for Node.js
ii  node-lru-cache                 2.3.1-1               all          least-recently-used cache object for Node.js
ii  node-mime                      1.2.11-1              all          library for mime-type mapping for Node.js
ii  node-minimatch                 0.2.12-1              all          Convert glob expressions into RegExp objects for Node.js
ii  node-mkdirp                    0.3.5-1               all          Node.js module to recursively create directories
ii  node-mute-stream               0.0.3-1               all          Pass-through stream that can be muted module for Node.js
ii  node-node-uuid                 1.4.0-1               all          simple, fast generation of RFC4122 UUIDs - Node module
ii  node-nopt                      2.1.2-1               all          Command-line option parser for Node.js
ii  node-normalize-package-data    0.2.2-1               all          Normalizes package metadata - Node.js module
ii  node-npmlog                    0.0.4-1               all          Logger with custom levels and colored output for Node.js
ii  node-once                      1.1.1-1               all          Run a function only once with this module for Node.js
ii  node-osenv                     0.0.3-1               all          Environment settings lookup module for Node.js
ii  node-qs                        0.6.5-1               all          querystring parser library for Node.js
ii  node-read                      1.0.4-1               all          Read user input from stdin module for Node.js
ii  node-read-package-json         1.1.3-1               all          Read package.json for npm module for Node.js
ii  node-request                   2.26.1-1              all          simplified HTTP request client module for Node.js
ii  node-retry                     0.6.0-1               all          Retry strategies for failed operations module for Node.js
ii  node-rimraf                    2.2.2-2               all          Deep deletion (like rm -rf) module for Node.js
ii  node-semver                    2.1.0-2               all          Semantic Versioning for Node.js
ii  node-sha                       1.2.3-1               all          Check and get file or stream hashes - module for Node.js
ii  node-sigmund                   1.0.0-1               all          Quick and dirty signatures for Objects module for Node.js
ii  node-slide                     1.1.4-1               all          Simple chain and asyncMap flow control module for Node.js
ii  node-tar                       0.1.18-1              all          read and write portable tar archives module for Node.js
ii  node-tunnel-agent              0.3.1-1               all          HTTP proxy tunneling agent module for Node.js
ii  node-which                     1.0.5-2               all          Cross-platform 'which' module for Node.js
ii  nodejs                         0.10.29~dfsg-1        armel        evented I/O for V8 javascript
ii  nodejs-dev                     0.10.29~dfsg-1        armel        evented I/O for V8 javascript (development files)
ii  npm                            1.4.4+ds-1            all          package manager for Node.js
ii  ntp                            1:4.2.6.p5+dfsg-3     armel        Network Time Protocol daemon and utility programs
ii  odbcinst                       2.3.1-3               armel        Helper program for accessing odbc ini files
ii  odbcinst1debian2:armel         2.3.1-3               armel        Support library for accessing odbc ini files
ii  openssh-client                 1:6.6p1-6             armel        secure shell (SSH) client, for secure access to remote machines
ii  openssh-server                 1:6.6p1-6             armel        secure shell (SSH) server, for secure access from remote machines
ii  openssh-sftp-server            1:6.6p1-6             armel        secure shell (SSH) sftp server module, for SFTP access from remote machines
ii  openssl                        1.0.1h-3              armel        Secure Sockets Layer toolkit - cryptographic utility
ii  parted                         2.3-20                armel        disk partition manipulator
ii  passwd                         1:4.2-2               armel        change and administer password and group data
ii  perl                           5.18.2-4              armel        Larry Wall's Practical Extraction and Report Language
ii  perl-base                      5.18.2-4              armel        minimal Perl system
ii  perl-modules                   5.18.2-4              all          Core Perl modules
ii  plymouth                       0.9.0-4               armel        Graphical Boot Animation and Logger
ii  policykit-1                    0.105-6               armel        framework for managing administrative policies and privileges
ii  procps                         1:3.3.9-5             armel        /proc file system utilities
ii  proj-data                      4.8.0-5               armel        Cartographic projection filter and library (datum package)
ii  psmisc                         22.21-2               armel        utilities that use the proc file system
ii  python                         2.7.6-2               armel        interactive high-level object-oriented language (default version)
ii  python-dbus                    1.2.0-2+b3            armel        simple interprocess messaging system (Python interface)
ii  python-dbus-dev                1.2.0-2               all          main loop integration development files for python-dbus
ii  python-gi                      3.12.1-1+b1           armel        Python 2.x bindings for gobject-introspection libraries
ii  python-gobject                 3.12.1-1              all          Python 2.x bindings for GObject - transitional package
ii  python-gobject-2               2.28.6-12             armel        deprecated static Python bindings for the GObject library
ii  python-minimal                 2.7.6-2               armel        minimal subset of the Python language (default version)
ii  python-pkg-resources           5.3-1                 all          Package Discovery and Resource Access using pkg_resources
ii  python-pyudev                  0.16.1-2              all          Python bindings for libudev
ii  python2.7                      2.7.8-1               armel        Interactive high-level object-oriented language (version 2.7)
ii  python2.7-minimal              2.7.8-1               armel        Minimal subset of the Python language (version 2.7)
ii  raspell                        1.3-1+b2              armel        interface binding for the Aspell spelling checker
ii  readline-common                6.3-6                 all          GNU readline and history libraries, common files
ii  rpcbind                        0.2.1-3               armel        converts RPC program numbers into universal addresses
ii  rsyslog                        7.6.3-3               armel        reliable system and kernel logging daemon
ii  ruby                           1:2.1.0.1             all          Interpreter of object-oriented scripting language Ruby (default version)
ii  ruby-augeas                    0.5.0-2+b2            armel        Augeas bindings for the Ruby language
ii  ruby-dbd-mysql                 0.4.4+gem2deb-1       all          Ruby/DBI MySQL driver
ii  ruby-dbd-pg                    0.3.9+gem2deb-1       all          Ruby/DBI PostgreSQL driver
ii  ruby-dbi                       0.4.5-3               all          Database Independent Interface for Ruby
ii  ruby-debian                    0.3.8+b4              armel        ruby interface for dpkg
ii  ruby-deprecated                3.0.1-2               all          Library for handling deprecated code in Ruby
ii  ruby-erubis                    2.7.0-3               all          fast and extensible eRuby implementation which supports multi-language
ii  ruby-extlib                    0.9.15-3              all          general Ruby class extensions for DataMapper and Merb
ii  ruby-fast-xs                   0.8.0-3+b3            armel        ruby extension for escaping text
ii  ruby-fcgi                      0.9.2.1-1+b2          armel        FastCGI library for Ruby
ii  ruby-flexmock                  0.9.0-1               all          simple and flexible mock objects for testing
ii  ruby-haml                      4.0.5-1               all          Elegant, structured XHTML/XML templating engine
ii  ruby-hdfeos5                   1.2-1+b2              armel        Ruby interface to the HDF-EOS5 library
ii  ruby-hdfeos5-dbg               1.2-1+b2              armel        Ruby interface to the HDF-EOS5 library (debug symbol)
ii  ruby-hpricot                   0.8.6-5+b2            armel        fast, enjoyable HTML parser
ii  ruby-htree                     0.8+dfsg-2            all          HTML/XML tree library for Ruby
ii  ruby-httpclient                2.3.3-3               all          HTTP client library for ruby (ruby 1.8 version)
ii  ruby-hyperestraier             1.4.13-13             armel        Hyper Estraier Node API Libraries for Ruby
ii  ruby-innate                    2013.02.21-1          all          core web-framework part of Ramaze
ii  ruby-json                      1.8.1-1+b1            armel        JSON library for Ruby
ii  ruby-liquid                    2.6.1-1               all          Ruby library for rendering safe HTML and email templates
ii  ruby-locale                    2.1.0-2               all          Locale library for Ruby
ii  ruby-mapscript                 6.4.1-4+b1            armel        MapServer library for Ruby
ii  ruby-maruku                    0.7.1-1               all          Markdown-superset interpreter written in Ruby
ii  ruby-mixlib-cli                1.4.0-1               all          Ruby mixin for creating command line applications
ii  ruby-mustache                  0.99.4-4              all          Mustache is a framework-agnostic way to render logic-free views
ii  ruby-mysql                     2.8.2+gem2deb-4+b2    armel        MySQL module for Ruby
ii  ruby-net-scp                   1.1.1-2               all          pure ruby implementation of the SCP protocol
ii  ruby-net-ssh                   1:2.6.8-2             all          Ruby implementation of the SSH protocol
ii  ruby-nokogiri                  1.6.2.1+ds-1          armel        HTML, XML, SAX, and Reader parser for Ruby
ii  ruby-packet                    0.1.15-5              all          Ruby library for Event driven network programming (dependency package)
ii  ruby-pg                        0.17.1-1              armel        PostgreSQL interface for Ruby
ii  ruby-qdbm                      1.8.78-4              armel        QDBM Database Libraries for Ruby
ii  ruby-rack                      1.5.2-1               all          Modular Ruby webserver interface
ii  ruby-rack-protection           1.5.2-1               all          Protects against typical web attacks for Rack apps
ii  ruby-ramaze                    2012.12.08-3          all          Simple and modular web framework
ii  ruby-rdiscount                 2.1.7.1-1+b1          armel        Discount Markdown Processor for Ruby
ii  ruby-rrd                       1.4.8-1+b1            armel        time-series data storage and display system (Ruby interface)
ii  ruby-sass                      3.3.4+really.3.2.19-2 all          powerful but elegant CSS compiler that makes CSS fun again
ii  ruby-sequel                    4.11.0-1              all          Simple, flexible, and powerful SQL database access toolkit for Ruby
ii  ruby-sinatra                   1.4.5-1               all          Ruby web-development dressed in a DSL
ii  ruby-slim                      2.0.2-3               all          powerful (X)HTML templating engine with an elegant syntax
ii  ruby-svg-graph                 1.0.5-2               all          Pure Ruby library for generating charts in SVG format
ii  ruby-temple                    0.6.7-1               all          template compilation framework in Ruby
ii  ruby-tilt                      2.0.0+really1.4.1-1   all          Generic interface to multiple Ruby template engines
ii  ruby-uconv                     0.6.1-1+b3            armel        Unicode/EUC-JP translation module for Ruby
ii  ruby-validatable               1.6.7-9               all          Ruby library for adding validations
ii  ruby-wirble                    0.1.3-4               all          Extensions for the Ruby irb command line shell
ii  ruby-zip                       1.1.2-1               armel        Ruby module for reading and writing zip files
ii  ruby2.1                        2.1.2-2               armel        Interpreter of object-oriented scripting language Ruby
ii  rubygems-integration           1.7                   all          integration of Debian Ruby packages with Rubygems
ii  sed                            4.2.2-4               armel        The GNU sed stream editor
ii  sensible-utils                 0.0.9                 all          Utilities for sensible alternative selection
ii  ssh                            1:6.6p1-6             all          secure shell client and server (metapackage)
ii  startpar                       0.59-3                armel        run processes in parallel and multiplex their output
ii  sudo                           1.8.9p5-1             armel        Provide limited super user privileges to specific users
ii  systemd                        204-14                armel        system and service manager
ii  systemd-sysv                   204-14                armel        system and service manager - SysV links
ii  sysv-rc                        2.88dsf-53.2          all          System-V-like runlevel change mechanism
ii  sysvinit                       2.88dsf-53.2          armel        System-V-like init utilities - metapackage
ii  sysvinit-utils                 2.88dsf-53.2          armel        System-V-like utilities
ii  tar                            1.27.1-2              armel        GNU version of the tar archiving utility
ii  tree                           1.7.0-1               armel        displays an indented directory tree, in color
ii  tzdata                         2014e-1               all          time zone and daylight-saving time data
ii  u-boot-tools                   2014.04+dfsg1-1       armel        companion tools for Das U-Boot bootloader
ii  ucf                            3.0030                all          Update Configuration File(s): preserve user changes to config files
ii  udev                           204-14                armel        /dev/ and hotplug management daemon
ii  unzip                          6.0-12                armel        De-archiver for .zip files
ii  usbutils                       1:007-2               armel        Linux USB utilities
ii  util-linux                     2.20.1-5.8            armel        Miscellaneous system utilities
ii  vim                            2:7.4.335-1           armel        Vi IMproved - enhanced vi editor
ii  vim-common                     2:7.4.335-1           armel        Vi IMproved - Common files
ii  vim-runtime                    2:7.4.335-1           all          Vi IMproved - Runtime files
ii  wget                           1.15-1+b1             armel        retrieves files from the web
ii  whiptail                       0.52.17-1             armel        Displays user-friendly dialog boxes from shell scripts
ii  wpasupplicant                  1.1-1                 armel        client support for WPA and WPA2 (IEEE 802.11i)
ii  xkb-data                       2.12-1                all          X Keyboard Extension (XKB) configuration data
ii  zip                            3.0-8                 armel        Archiver for .zip files
ii  zlib1g:armel                   1:1.2.8.dfsg-1        armel        compression library - runtime
ii  zlib1g-dev:armel               1:1.2.8.dfsg-1        armel        compression library - development
```
