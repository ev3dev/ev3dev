Release notes for ev3dev-jessie-2014-10-07.img
==============================================

Changes from previous version
-----------------------------
* Remove ev3dev.rc.local
* Includes Brick Manager (brickman)
* Includes ralink-firmware
* Uses ConnMan instead of NetworkManager
* Got rid of package pinning in favor of aptdefaultrelease
* Use default ruby package instead of ruby1.9.1
* Remove bluez-tools package
* Input port 1 is enabled for sensors by default
* Fixed issue with sudoers file
* SSH sessions terminate properly (most of the time)
* journald is set for persistant storage
* Can now configure kernel command line

Known issues
------------
* `plymouth` is not working during boot/shutdown.

Built using
-----------
* elementary OS Freya
* brickstrap 0.2.6
* multistrap 2.2.0ubuntu2
* proot 3.2.2-1ev3dev2
* libguestfs-tools 1:1.24.5-1ev3dev1

Included Packages
-----------------

```
Desired=Unknown/Install/Remove/Purge/Hold
| Status=Not/Inst/Conf-files/Unpacked/halF-conf/Half-inst/trig-aWait/Trig-pend
|/ Err?=(none)/Reinst-required (Status,Err: uppercase=bad)
||/ Name                              Version                        Architecture Description
+++-=================================-==============================-============-===============================================================================
ii  acl                               2.2.52-2                       armel        Access control list utilities
ii  adduser                           3.113+nmu3                     all          add and remove users and groups
ii  alsa-utils                        1.0.28-1                       armel        Utilities for configuring and using ALSA
ii  apt                               1.0.9.2                        armel        commandline package manager
ii  base-files                        7.5ev3dev1                     armel        Debian base system miscellaneous files
ii  base-passwd                       3.5.36                         armel        Debian base system master password and group files
ii  bash                              4.3-10                         armel        GNU Bourne Again SHell
ii  beep                              1.3-3+b1                       armel        advanced pc-speaker beeper
ii  bluez                             5.23-1                         armel        Bluetooth tools and daemons
ii  brickman                          0.1.1                          armel        ev3dev Brick Manager
ii  bsdmainutils                      9.0.5                          armel        collection of more utilities from FreeBSD
ii  bsdutils                          1:2.20.1-5.11                  armel        Basic utilities from 4.4BSD-Lite
ii  ca-certificates                   20140325                       all          Common CA certificates
ii  connman                           1.25-0ev3dev1                  armel        Intel Connection Manager daemon
ii  console-setup                     1.113                          all          console font and keymap setup program
ii  console-setup-linux               1.113                          all          Linux specific part of console-setup
ii  conspy                            1.10-1                         armel        Remote control of Linux virtual consoles
ii  coreutils                         8.23-2                         armel        GNU core utilities
ii  cpio                              2.11+dfsg-2                    armel        GNU cpio -- a program to manage archives of files
ii  dash                              0.5.7-4                        armel        POSIX-compliant shell
ii  dbus                              1.8.8-1                        armel        simple interprocess messaging system (daemon and utilities)
ii  debconf                           1.5.53                         all          Debian configuration management system
ii  debian-archive-keyring            2014.1                         all          GnuPG archive keys of the Debian archive
ii  debianutils                       4.4                            armel        Miscellaneous utilities specific to Debian
ii  devio                             1.2-1+b1                       armel        correctly read (or write) a region of a block device
ii  dh-python                         1.20140511-1                   all          Debian helper tools for packaging Python libraries and applications
ii  diffutils                         1:3.3-1                        armel        File comparison utilities
ii  dmeventd                          2:1.02.90-2                    armel        Linux Kernel Device Mapper event daemon
ii  dmsetup                           2:1.02.90-2                    armel        Linux Kernel Device Mapper userspace library
ii  dosfstools                        3.0.26-3                       armel        utilities for making and checking MS-DOS FAT filesystems
ii  dpkg                              1.17.13                        armel        Debian package management system
ii  e2fslibs:armel                    1.42.12-1                      armel        ext2/ext3/ext4 file system libraries
ii  e2fsprogs                         1.42.12-1                      armel        ext2/ext3/ext4 file system utilities
ii  espeak                            1.47.11-1ev3dev1               armel        Multi-lingual software speech synthesizer
ii  espeak-data:armel                 1.47.11-1ev3dev1               armel        Multi-lingual software speech synthesizer: speech data files
ii  ethtool                           1:3.16-1                       armel        display or change Ethernet device settings
ii  ev3dev-archive-keyring            0                              all          GnuPG archive keys of the ev3dev archive
ii  ev3dev-base                       7.4                            armel        Meta package that installs all of the required ev3dev packages.
ii  ev3dev-bluetooth                  7.4                            armel        Firmware and scripts for EV3 bluetooth.
ii  ev3dev-console                    7.4                            armel        Console related configuration files and console fonts.
ii  ev3dev-flash-kernel               7.4                            armel        Database entry and boot script for flash-kernel.
ii  ev3dev-gadget                     7.4                            armel        systemd services for starting/stopping USB Ethernet gadget modules.
ii  ev3dev-i2c                        7.4                            armel        Udev rules for I2C devices.
ii  ev3dev-leds                       7.4                            armel        Initialization scripts for EV3 LEDs.
ii  ev3dev-ports                      7.4                            armel        Scripts related to the EV3 input and output ports
ii  ev3dev-uart                       7.4                            armel        Firmware and scripts for EV3 input port UARTs.
ii  fbcat                             0.3-1ev3dev1                   armel        framebuffer grabber
ii  findutils                         4.4.2-9                        armel        utilities for finding files--find, xargs
ii  firmware-atheros                  0.43                           all          Binary firmware for Atheros wireless cards
ii  firmware-ralink                   0.43                           all          Binary firmware for Ralink wireless cards
ii  firmware-realtek                  0.43                           all          Binary firmware for Realtek wired and wireless network adapters
ii  flash-kernel                      3.25                           armel        utility to make certain embedded devices bootable
ii  gawk                              1:4.1.1+dfsg-1                 armel        GNU awk, a pattern scanning and processing language
ii  gcc-4.7-base:armel                4.7.4-3                        armel        GCC, the GNU Compiler Collection (base package)
ii  gcc-4.8-base:armel                4.8.3-11                       armel        GCC, the GNU Compiler Collection (base package)
ii  gcc-4.9-base:armel                4.9.1-16                       armel        GCC, the GNU Compiler Collection (base package)
ii  gir1.2-glib-2.0:armel             1.42.0-1                       armel        Introspection data for GLib, GObject, Gio and GModule
ii  gnupg                             1.4.18-4                       armel        GNU privacy guard - a free PGP replacement
ii  golang-go                         2:1.3.2-1                      armel        Go programming language compiler
ii  golang-go-linux-arm               2:1.3.2-1                      armel        Go standard library compiled for linux_arm
ii  golang-src                        2:1.3.2-1                      armel        Go programming language compiler - source files
ii  gpgv                              1.4.18-4                       armel        GNU privacy guard - signature verification tool
ii  grep                              2.20-3                         armel        GNU grep, egrep and fgrep
ii  guile-1.8                         1.8.8+1-9                      armel        GNU extension language and Scheme interpreter
ii  guile-1.8-libs                    1.8.8+1-9                      armel        Core Guile libraries
ii  gyp                               0.1~svn1729-3                  all          Cross-platform build script generator
ii  gzip                              1.6-3                          armel        GNU compression utilities
ii  hostname                          3.15                           armel        utility to set/show the host name or domain name
ii  ifupdown                          0.7.49                         armel        high level tools to configure network interfaces
ii  init                              1.21                           armel        System-V-like init utilities - metapackage
ii  init-system-helpers               1.21                           all          helper tools for all init systems
ii  initramfs-tools                   0.116                          all          generic modular initramfs generator
ii  initscripts                       2.88dsf-53.4                   armel        scripts for initializing and shutting down the system
ii  insserv                           1.14.0-5                       armel        boot sequence organizer using LSB init.d script dependency information
ii  iproute                           1:3.16.0-2                     all          transitional dummy package for iproute2
ii  iproute2                          3.16.0-2                       armel        networking and traffic control tools
ii  iputils-ping                      3:20121221-5+b1                armel        Tools to test the reachability of network hosts
ii  isc-dhcp-client                   4.3.1-1                        armel        ISC DHCP client
ii  isc-dhcp-common                   4.3.1-1                        armel        common files used by all of the isc-dhcp packages
ii  kbd                               1.15.5-1                       armel        Linux console font and keytable utilities
ii  keyboard-configuration            1.113                          all          system-wide keyboard preferences
ii  klibc-utils                       2.0.4-1.1                      armel        small utilities built with klibc for early boot
ii  kmod                              18-3                           armel        tools for managing Linux kernel modules
ii  less                              458-3                          armel        pager program similar to more
ii  libacl1:armel                     2.2.52-2                       armel        Access control list shared library
ii  libapt-pkg4.12:armel              1.0.9.2                        armel        package management runtime library
ii  libasn1-8-heimdal:armel           1.6~rc2+dfsg-8                 armel        Heimdal Kerberos - ASN.1 library
ii  libasound2:armel                  1.0.28-1                       armel        shared library for ALSA applications
ii  libasound2-data                   1.0.28-1                       all          Configuration files and profiles for ALSA drivers
ii  libattr1:armel                    1:2.4.47-2                     armel        Extended attribute shared library
ii  libaudit-common                   1:2.4-1                        all          Dynamic library for security auditing - common files
ii  libaudit1:armel                   1:2.4-1                        armel        Dynamic library for security auditing
ii  libavahi-client3:armel            0.6.31-4                       armel        Avahi client library
ii  libavahi-common-data:armel        0.6.31-4                       armel        Avahi common data files
ii  libavahi-common3:armel            0.6.31-4                       armel        Avahi common library
ii  libblkid1:armel                   2.20.1-5.11                    armel        block device id library
ii  libbsd0:armel                     0.7.0-2                        armel        utility functions from BSD systems - shared library
ii  libbz2-1.0:armel                  1.0.6-7                        armel        high-quality block-sorting file compressor library - runtime
ii  libc-ares-dev:armel               1.10.0-2                       armel        asynchronous name resolver - development files
ii  libc-ares2:armel                  1.10.0-2                       armel        asynchronous name resolver
ii  libc-bin                          2.19-11                        armel        GNU C Library: Binaries
ii  libc-dev-bin                      2.19-11                        armel        GNU C Library: Development binaries
ii  libc6:armel                       2.19-11                        armel        GNU C Library: Shared libraries
ii  libc6-dev:armel                   2.19-11                        armel        GNU C Library: Development Libraries and Header Files
ii  libcap-ng0:armel                  0.7.4-2                        armel        An alternate POSIX capabilities library
ii  libcap2:armel                     1:2.24-6                       armel        POSIX 1003.1e capabilities (library)
ii  libcap2-bin                       1:2.24-6                       armel        POSIX 1003.1e capabilities (utilities)
ii  libcomerr2:armel                  1.42.12-1                      armel        common error description library
ii  libcryptsetup4:armel              2:1.6.6-1                      armel        disk encryption support - shared library
ii  libcups2:armel                    1.7.5-1                        armel        Common UNIX Printing System(tm) - Core library
ii  libdb5.3:armel                    5.3.28-6                       armel        Berkeley v5.3 Database Libraries [runtime]
ii  libdbus-1-3:armel                 1.8.8-1                        armel        simple interprocess messaging system (library)
ii  libdebconfclient0:armel           0.192                          armel        Debian Configuration Management System (C-implementation library)
ii  libdevmapper-event1.02.1:armel    2:1.02.90-2                    armel        Linux Kernel Device Mapper event support library
ii  libdevmapper1.02.1:armel          2:1.02.90-2                    armel        Linux Kernel Device Mapper userspace library
ii  libdrm2:armel                     2.4.56-1                       armel        Userspace interface to kernel DRM services -- runtime
ii  libedit2:armel                    3.1-20140620-2                 armel        BSD editline and history libraries
ii  libespeak1:armel                  1.47.11-1ev3dev1               armel        Multi-lingual software speech synthesizer: shared library
ii  libevent-2.0-5:armel              2.0.21-stable-1.1              armel        Asynchronous event notification library
ii  libexpat1:armel                   2.1.0-6                        armel        XML parsing C library - runtime library
ii  libffi6:armel                     3.1-2                          armel        Foreign Function Interface library runtime
ii  libfuse2:armel                    2.9.3-15                       armel        Filesystem in Userspace (library)
ii  libgcc1:armel                     1:4.9.1-16                     armel        GCC support library
ii  libgcrypt11:armel                 1.5.4-3                        armel        LGPL Crypto library - runtime library
ii  libgcrypt20:armel                 1.6.2-3                        armel        LGPL Crypto library - runtime library
ii  libgdbm3:armel                    1.8.3-13                       armel        GNU dbm database routines (runtime version)
ii  libgee-0.8-2:armel                0.14.0-3                       armel        GObject based collection and utility library
ii  libgirepository-1.0-1:armel       1.42.0-1                       armel        Library for handling GObject introspection data (runtime library)
ii  libglib2.0-0:armel                2.42.0-1                       armel        GLib library of C routines
ii  libgmp10:armel                    2:6.0.0+dfsg-6                 armel        Multiprecision arithmetic library
ii  libgnome-keyring-common           3.12.0-1                       all          GNOME keyring services library - data files
ii  libgnome-keyring0:armel           3.12.0-1                       armel        GNOME keyring services library
ii  libgnutls-deb0-28:armel           3.3.8-2                        armel        GNU TLS library - main runtime library
ii  libgnutls-openssl27:armel         3.3.8-2                        armel        GNU TLS library - OpenSSL wrapper
ii  libgnutls26:armel                 2.12.23-17                     armel        GNU TLS library - runtime library
ii  libgpg-error0:armel               1.16-2                         armel        library for common error values and messages in GnuPG components
ii  libgpm2:armel                     1.20.4-6.1                     armel        General Purpose Mouse - shared library
ii  libgrx-fonts                      2.4.9-0ev3dev1                 all          2D graphics library
ii  libgrx20-2                        2.4.9-0ev3dev1                 armel        2D graphics library
ii  libgssapi-krb5-2:armel            1.12.1+dfsg-10                 armel        MIT Kerberos runtime libraries - krb5 GSS-API Mechanism
ii  libgssapi3-heimdal:armel          1.6~rc2+dfsg-8                 armel        Heimdal Kerberos - GSSAPI support library
ii  libgudev-1.0-0:armel              215-5+b1                       armel        GObject-based wrapper library for libudev
ii  libhcrypto4-heimdal:armel         1.6~rc2+dfsg-8                 armel        Heimdal Kerberos - crypto library
ii  libheimbase1-heimdal:armel        1.6~rc2+dfsg-8                 armel        Heimdal Kerberos - Base library
ii  libheimntlm0-heimdal:armel        1.6~rc2+dfsg-8                 armel        Heimdal Kerberos - NTLM support library
ii  libhogweed2:armel                 2.7.1-3                        armel        low level cryptographic library (public-key cryptos)
ii  libhx509-5-heimdal:armel          1.6~rc2+dfsg-8                 armel        Heimdal Kerberos - X509 support library
ii  libidn11:armel                    1.29-1                         armel        GNU Libidn library, implementation of IETF IDN specifications
ii  libjbig0:armel                    2.1-3                          armel        JBIGkit libraries
ii  libjpeg62:armel                   1:1.3.1-3                      armel        LJT JPEG runtime library
ii  libjs-node-uuid                   1.4.0-1                        all          simple, fast generation of RFC4122 UUIDs - JavaScript library
ii  libjs-underscore                  1.4.4-2                        all          JavaScript's functional programming helper library
ii  libk5crypto3:armel                1.12.1+dfsg-10                 armel        MIT Kerberos runtime libraries - Crypto Library
ii  libkeyutils1:armel                1.5.9-5                        armel        Linux Key Management Utilities (library)
ii  libklibc                          2.0.4-1.1                      armel        minimal libc subset for use with initramfs
ii  libkmod2:armel                    18-3                           armel        libkmod shared library
ii  libkrb5-26-heimdal:armel          1.6~rc2+dfsg-8                 armel        Heimdal Kerberos - libraries
ii  libkrb5-3:armel                   1.12.1+dfsg-10                 armel        MIT Kerberos runtime libraries
ii  libkrb5support0:armel             1.12.1+dfsg-10                 armel        MIT Kerberos runtime libraries - Support library
ii  libldap-2.4-2:armel               2.4.39-1.1                     armel        OpenLDAP libraries
ii  libldb1:armel                     1:1.1.17-1                     armel        LDAP-like embedded database - shared library
ii  liblocale-gettext-perl            1.05-8+b1                      armel        module using libc functions for internationalization in Perl
ii  libltdl7:armel                    2.4.2-1.10                     armel        System independent dlopen wrapper for GNU libtool
ii  liblvm2cmd2.02:armel              2.02.111-2                     armel        LVM2 command library
ii  liblzma5:armel                    5.1.1alpha+20120614-2          armel        XZ-format compression library
ii  libmount1                         2.20.1-5.11                    armel        block device id library
ii  libmpdec2:armel                   2.4.1-1                        armel        library for decimal floating point arithmetic (runtime library)
ii  libmpfr4:armel                    3.1.2-1                        armel        multiple precision floating-point computation
ii  libncurses5:armel                 5.9+20140913-1                 armel        shared libraries for terminal handling
ii  libncursesw5:armel                5.9+20140913-1                 armel        shared libraries for terminal handling (wide character support)
ii  libnetpbm10                       2:10.0-15+b3                   armel        Graphics conversion tools shared libraries
ii  libnettle4:armel                  2.7.1-3                        armel        low level cryptographic library (symmetric and one-way cryptos)
ii  libnewt0.52:armel                 0.52.17-1                      armel        Not Erik's Windowing Toolkit - text mode windowing with slang
ii  libnfsidmap2:armel                0.25-5                         armel        NFS idmapping library
ii  libnl-3-200:armel                 3.2.24-2                       armel        library for dealing with netlink sockets
ii  libnl-genl-3-200:armel            3.2.24-2                       armel        library for dealing with netlink sockets - generic netlink
ii  libntdb1:armel                    1.0-5                          armel        New Trivial Database - shared library
ii  libopts25:armel                   1:5.18.4-2                     armel        automated option processing library based on autogen
ii  libp11-kit0:armel                 0.20.7-1                       armel        Library for loading and coordinating access to PKCS#11 modules - runtime
ii  libpam-modules:armel              1.1.8-3.1                      armel        Pluggable Authentication Modules for PAM
ii  libpam-modules-bin                1.1.8-3.1                      armel        Pluggable Authentication Modules for PAM - helper binaries
ii  libpam-runtime                    1.1.8-3.1                      all          Runtime support for the PAM library
ii  libpam0g:armel                    1.1.8-3.1                      armel        Pluggable Authentication Modules library
ii  libparted2:armel                  3.2-6                          armel        disk partition manipulator - shared library
ii  libpcre3:armel                    1:8.35-3                       armel        Perl 5 Compatible Regular Expression Library - runtime files
ii  libpcsclite1:armel                1.8.12-1                       armel        Middleware to access a smart card using PC/SC (library)
ii  libpng12-0:armel                  1.2.50-2                       armel        PNG library - runtime
ii  libpopt0:armel                    1.16-10                        armel        lib for parsing cmdline parameters
ii  libprocps3:armel                  2:3.3.9-8                      armel        library for accessing process information from /proc
ii  libpython-stdlib:armel            2.7.8-1                        armel        interactive high-level object-oriented language (default python version)
ii  libpython2.7:armel                2.7.8-7                        armel        Shared Python runtime library (version 2.7)
ii  libpython2.7-minimal:armel        2.7.8-7                        armel        Minimal subset of the Python language (version 2.7)
ii  libpython2.7-stdlib:armel         2.7.8-7                        armel        Interactive high-level object-oriented language (standard library, version 2.7)
ii  libpython3-stdlib:armel           3.4.1-1                        armel        interactive high-level object-oriented language (default python3 version)
ii  libpython3.4-minimal:armel        3.4.2~rc1-1                    armel        Minimal subset of the Python language (version 3.4)
ii  libpython3.4-stdlib:armel         3.4.2~rc1-1                    armel        Interactive high-level object-oriented language (standard library, version 3.4)
ii  libreadline5:armel                5.2+dfsg-2                     armel        GNU readline and history libraries, run-time libraries
ii  libreadline6:armel                6.3-8                          armel        GNU readline and history libraries, run-time libraries
ii  libroken18-heimdal:armel          1.6~rc2+dfsg-8                 armel        Heimdal Kerberos - roken support library
ii  libruby2.1:armel                  2.1.3-1                        armel        Libraries necessary to run Ruby 2.1
ii  libsamplerate0:armel              0.1.8-8                        armel        Audio sample rate conversion library
ii  libsasl2-2:armel                  2.1.26.dfsg1-11                armel        Cyrus SASL - authentication abstraction library
ii  libsasl2-modules-db:armel         2.1.26.dfsg1-11                armel        Cyrus SASL - pluggable authentication modules (DB)
ii  libselinux1:armel                 2.3-2                          armel        SELinux runtime shared libraries
ii  libsemanage-common                2.3-1                          all          Common files for SELinux policy management libraries
ii  libsemanage1:armel                2.3-1                          armel        SELinux policy management library
ii  libsepol1:armel                   2.3-2                          armel        SELinux library for manipulating binary security policies
ii  libsigsegv2:armel                 2.10-4                         armel        Library for handling page faults in a portable way
ii  libslang2:armel                   2.3.0-1                        armel        S-Lang programming library - runtime version
ii  libsmbclient:armel                2:4.1.11+dfsg-1                armel        shared library for communication with SMB/CIFS servers
ii  libsonic0:armel                   0.1.17-1.1                     armel        Simple library to speed up or slow down speech
ii  libsqlite3-0:armel                3.8.6-1                        armel        SQLite 3 shared library
ii  libss2:armel                      1.42.12-1                      armel        command-line interface parsing library
ii  libssl-dev:armel                  1.0.1i-2                       armel        Secure Sockets Layer toolkit - development files
ii  libssl1.0.0:armel                 1.0.1i-2                       armel        Secure Sockets Layer toolkit - shared libraries
ii  libstdc++6:armel                  4.9.1-16                       armel        GNU Standard C++ Library v3
ii  libsystemd0:armel                 215-5+b1                       armel        systemd utility library
ii  libtalloc2:armel                  2.1.1-2                        armel        hierarchical pool based memory allocator
ii  libtasn1-6:armel                  4.2-1                          armel        Manage ASN.1 structures (runtime)
ii  libtdb1:armel                     1.3.1-1                        armel        Trivial Database - shared library
ii  libtevent0:armel                  0.9.21-1                       armel        talloc-based event loop library - shared library
ii  libtext-charwidth-perl            0.04-7+b3                      armel        get display widths of characters on the terminal
ii  libtext-iconv-perl                1.7-5+b2                       armel        converts between character sets in Perl
ii  libtext-wrapi18n-perl             0.06-7                         all          internationalized substitute of Text::Wrap
ii  libtiff5:armel                    4.0.3-10+b1                    armel        Tag Image File Format (TIFF) library
ii  libtinfo5:armel                   5.9+20140913-1                 armel        shared low-level terminfo library for terminal handling
ii  libtirpc1:armel                   0.2.5-1                        armel        transport-independent RPC library
ii  libudev1:armel                    215-5+b1                       armel        libudev shared library
ii  libusb-0.1-4:armel                2:0.1.12-24                    armel        userspace USB programming library
ii  libusb-1.0-0:armel                2:1.0.19-1                     armel        userspace USB programming library
ii  libustr-1.0-1:armel               1.0.4-3                        armel        Micro string library: shared library
ii  libuuid-perl                      0.05-1+b1                      armel        Perl extension for using UUID interfaces as defined in e2fsprogs
ii  libuuid1:armel                    2.20.1-5.11                    armel        Universally Unique ID library
ii  libv8-3.14-dev                    3.14.5.8-8                     armel        V8 JavaScript engine - development files for 3.14 branch
ii  libv8-3.14.5                      3.14.5.8-8                     armel        V8 JavaScript engine - runtime library
ii  libwbclient0:armel                2:4.1.11+dfsg-1                armel        Samba winbind client library
ii  libwind0-heimdal:armel            1.6~rc2+dfsg-8                 armel        Heimdal Kerberos - stringprep implementation
ii  libwrap0:armel                    7.6.q-25                       armel        Wietse Venema's TCP wrappers library
ii  libxtables10                      1.4.21-2                       armel        netfilter xtables library
ii  libyaml-0-2:armel                 0.1.6-2                        armel        Fast YAML 1.1 parser and emitter library
ii  linux-base                        3.5                            all          Linux image base package
ii  linux-image-3.16.1-4-ev3dev       1                              armel        Linux kernel binary image for version 3.16.1-4-ev3dev
ii  linux-image-ev3dev                10                             armel        Linux kernel for ev3dev (meta-package)
ii  linux-libc-dev:armel              3.16.3-2                       armel        Linux support headers for userspace development
ii  locales                           2.19-11                        all          GNU C Library: National Language (locale) data [support]
ii  login                             1:4.2-2+b1                     armel        system login tools
ii  lsb-base                          4.1+Debian13                   all          Linux Standard Base 4.1 init script functionality
ii  lua5.1                            5.1.5-7                        armel        Simple, extensible, embeddable programming language
ii  lvm2                              2.02.111-2                     armel        Linux Logical Volume Manager
ii  mawk                              1.3.3-17                       armel        a pattern scanning and text processing language
ii  mime-support                      3.56                           all          MIME files 'mime.types' & 'mailcap', and support programs
ii  mount                             2.20.1-5.11                    armel        Tools for mounting and manipulating filesystems
ii  multiarch-support                 2.19-11                        armel        Transitional package to ensure multiarch compatibility
ii  nano                              2.2.6-3                        armel        small, friendly text editor inspired by Pico
ii  ncurses-base                      5.9+20140913-1                 all          basic terminal type definitions
ii  ncurses-bin                       5.9+20140913-1                 armel        terminal-related programs and man pages
ii  net-tools                         1.60-26                        armel        NET-3 networking toolkit
ii  netbase                           5.2                            all          Basic TCP/IP networking system
ii  netcat-openbsd                    1.105-7                        armel        TCP/IP swiss army knife
ii  netpbm                            2:10.0-15+b3                   armel        Graphics conversion tools between image formats
ii  nfs-common                        1:1.2.8-9                      armel        NFS support files common to client and server
ii  node-abbrev                       1.0.5-2                        all          Get unique abbreviations for a set of strings - Node.js module
ii  node-ansi                         0.3.0-2                        all          Advanced ANSI formatting tool for Node.js
ii  node-ansi-color-table             1.0.0-1                        all          Color and format tables for ansi output - Node.js module
ii  node-archy                        0.0.2-1                        all          Pretty-print nested hierarchies module for Node.js
ii  node-async                        0.8.0-1                        all          higher-order functions and common patterns for asynchronous Javascript
ii  node-block-stream                 0.0.7-1                        all          Stream of fixed-size blocks, with zero-padding when necessary
ii  node-combined-stream              0.0.5-1                        all          Append streams one after another - module for Node.js
ii  node-cookie-jar                   0.3.1-1                        all          Cookie handling for HTTP clients - module for Node.js
ii  node-delayed-stream               0.0.5-1                        all          Buffer stream events for later handling - module for Node.js
ii  node-forever-agent                0.5.1-1                        all          HTTP agent supporting keep-alive requests - module for Node.js
ii  node-form-data                    0.1.0-1                        all          Create multipart/form-data streams module for Node.js
ii  node-fstream                      0.1.24-1                       all          Advanced filesystem streaming tools for Node.js
ii  node-fstream-ignore               0.0.6-2                        all          Directory reader configurable by .ignore module for Node.js
ii  node-github-url-from-git          1.1.1-1                        all          Convert github git or gist url to an http url - Node.js module
ii  node-glob                         4.0.5-1                        all          glob functionality for Node.js
ii  node-graceful-fs                  3.0.2-1                        all          drop-in replacement improving the Node.js fs module
ii  node-gyp                          0.12.2+ds-1                    all          Native addon build tool for Node.js
ii  node-inherits                     2.0.0-1                        all          Exposes inherits function from Node.js environment
ii  node-ini                          1.1.0-1                        all          ini format parser and serializer for Node.js
ii  node-json-stringify-safe          5.0.0-1                        all          JSON.stringify with circular references module for Node.js
ii  node-lockfile                     0.4.1-1                        all          Asynchronous file lock module for Node.js
ii  node-lru-cache                    2.3.1-1                        all          least-recently-used cache object for Node.js
ii  node-mime                         1.2.11-1                       all          library for mime-type mapping for Node.js
ii  node-minimatch                    1.0.0-1                        all          Convert glob expressions into RegExp objects for Node.js
ii  node-mkdirp                       0.5.0-1                        all          Recursively create directories - Node.js module
ii  node-mute-stream                  0.0.4-1                        all          Pass-through stream that can be muted module for Node.js
ii  node-node-uuid                    1.4.0-1                        all          simple, fast generation of RFC4122 UUIDs - Node module
ii  node-nopt                         3.0.1-1                        all          Command-line option parser for Node.js
ii  node-normalize-package-data       0.2.2-1                        all          Normalizes package metadata - Node.js module
ii  node-npmlog                       0.0.4-1                        all          Logger with custom levels and colored output for Node.js
ii  node-once                         1.1.1-1                        all          Run a function only once with this module for Node.js
ii  node-osenv                        0.1.0-1                        all          Environment settings lookup module for Node.js
ii  node-qs                           0.6.5-1                        all          querystring parser library for Node.js
ii  node-read                         1.0.5-1                        all          Read user input from stdin module for Node.js
ii  node-read-package-json            1.2.4-1                        all          Read package.json for npm module for Node.js
ii  node-request                      2.26.1-1                       all          simplified HTTP request client module for Node.js
ii  node-retry                        0.6.0-1                        all          Retry strategies for failed operations module for Node.js
ii  node-rimraf                       2.2.8-1                        all          Deep deletion (like rm -rf) module for Node.js
ii  node-semver                       2.1.0-2                        all          Semantic Versioning for Node.js
ii  node-sha                          1.2.3-1                        all          Check and get file or stream hashes - module for Node.js
ii  node-sigmund                      1.0.0-1                        all          Quick and dirty signatures for Objects module for Node.js
ii  node-slide                        1.1.4-1                        all          Simple chain and asyncMap flow control module for Node.js
ii  node-tar                          0.1.18-1                       all          read and write portable tar archives module for Node.js
ii  node-tunnel-agent                 0.3.1-1                        all          HTTP proxy tunneling agent module for Node.js
ii  node-underscore                   1.4.4-2                        all          JavaScript's functional programming helper library - NodeJS
ii  node-which                        1.0.5-2                        all          Cross-platform 'which' module for Node.js
ii  nodejs                            0.10.29~dfsg-1                 armel        evented I/O for V8 javascript
ii  nodejs-dev                        0.10.29~dfsg-1                 armel        evented I/O for V8 javascript (development files)
ii  npm                               1.4.21+ds-2                    all          package manager for Node.js
ii  ntp                               1:4.2.6.p5+dfsg-3.1            armel        Network Time Protocol daemon and utility programs
ii  openssh-client                    1:6.6p1-7                      armel        secure shell (SSH) client, for secure access to remote machines
ii  openssh-server                    1:6.6p1-7                      armel        secure shell (SSH) server, for secure access from remote machines
ii  openssh-sftp-server               1:6.6p1-7                      armel        secure shell (SSH) sftp server module, for SFTP access from remote machines
ii  openssl                           1.0.1i-2                       armel        Secure Sockets Layer toolkit - cryptographic utility
ii  parted                            3.2-6                          armel        disk partition manipulator
ii  passwd                            1:4.2-2+b1                     armel        change and administer password and group data
ii  perl                              5.20.1-1                       armel        Larry Wall's Practical Extraction and Report Language
ii  perl-base                         5.20.1-1                       armel        minimal Perl system
ii  perl-modules                      5.20.1-1                       all          Core Perl modules
ii  plymouth                          0.9.0-7ev3dev1                 armel        Graphical Boot Animation and Logger
ii  procps                            2:3.3.9-8                      armel        /proc file system utilities
ii  psmisc                            22.21-2                        armel        utilities that use the proc file system
ii  python                            2.7.8-1                        armel        interactive high-level object-oriented language (default version)
ii  python-gi                         3.14.0-1                       armel        Python 2.x bindings for gobject-introspection libraries
ii  python-gobject                    3.14.0-1                       all          Python 2.x bindings for GObject - transitional package
ii  python-gobject-2                  2.28.6-12                      armel        deprecated static Python bindings for the GObject library
ii  python-minimal                    2.7.8-1                        armel        minimal subset of the Python language (default version)
ii  python-pkg-resources              5.5.1-1                        all          Package Discovery and Resource Access using pkg_resources
ii  python-pyudev                     0.16.1-2                       all          Python bindings for libudev
ii  python-talloc                     2.1.1-2                        armel        hierarchical pool based memory allocator - Python bindings
ii  python2.7                         2.7.8-7                        armel        Interactive high-level object-oriented language (version 2.7)
ii  python2.7-minimal                 2.7.8-7                        armel        Minimal subset of the Python language (version 2.7)
ii  python3                           3.4.1-1                        armel        interactive high-level object-oriented language (default python3 version)
ii  python3-minimal                   3.4.1-1                        armel        minimal subset of the Python language (default python3 version)
ii  python3.4                         3.4.2~rc1-1                    armel        Interactive high-level object-oriented language (version 3.4)
ii  python3.4-minimal                 3.4.2~rc1-1                    armel        Minimal subset of the Python language (version 3.4)
ii  readline-common                   6.3-8                          all          GNU readline and history libraries, common files
ii  rpcbind                           0.2.1-6                        armel        converts RPC program numbers into universal addresses
ii  rtl8188eu-modules-3.16.1-4-ev3dev 3+1                            armel        rtl8188eu modules for Linux (kernel 3.16.1-4-ev3dev).
ii  rtl8192cu-modules-3.16.1-4-ev3dev 4.0.2-9000.20131029-0ev3dev1+1 armel        rtl8192cu series modules for Linux (kernel 3.16.1-4-ev3dev).
ii  ruby                              1:2.1.0.4                      all          Interpreter of object-oriented scripting language Ruby (default version)
ii  ruby2.1                           2.1.3-1                        armel        Interpreter of object-oriented scripting language Ruby
ii  rubygems-integration              1.8                            all          integration of Debian Ruby packages with Rubygems
ii  samba-libs:armel                  2:4.1.11+dfsg-1                armel        Samba core libraries
ii  sed                               4.2.2-4                        armel        The GNU sed stream editor
ii  sensible-utils                    0.0.9                          all          Utilities for sensible alternative selection
ii  smbnetfs                          0.5.3b-1                       armel        User-space filesystem for SMB/NMB (Windows) network servers and shares
ii  ssh                               1:6.6p1-7                      all          secure shell client and server (metapackage)
ii  startpar                          0.59-3                         armel        run processes in parallel and multiplex their output
ii  sudo                              1.8.10p3-1                     armel        Provide limited super user privileges to specific users
ii  systemd                           215-5+b1                       armel        system and service manager
ii  systemd-sysv                      215-5+b1                       armel        system and service manager - SysV links
ii  sysv-rc                           2.88dsf-53.4                   all          System-V-like runlevel change mechanism
ii  sysvinit                          2.88dsf-53.4                   armel        System-V-like init utilities - transitional package
ii  sysvinit-utils                    2.88dsf-53.4                   armel        System-V-like utilities
ii  tar                               1.27.1-2                       armel        GNU version of the tar archiving utility
ii  tree                              1.7.0-1                        armel        displays an indented directory tree, in color
ii  tzdata                            2014h-1                        all          time zone and daylight-saving time data
ii  u-boot-tools                      2014.07+dfsg1-2                armel        companion tools for Das U-Boot bootloader
ii  ucf                               3.0030                         all          Update Configuration File(s): preserve user changes to config files
ii  udev                              215-5+b1                       armel        /dev/ and hotplug management daemon
ii  usbutils                          1:007-2                        armel        Linux USB utilities
ii  util-linux                        2.20.1-5.11                    armel        Miscellaneous system utilities
ii  vim                               2:7.4.430-1                    armel        Vi IMproved - enhanced vi editor
ii  vim-common                        2:7.4.430-1                    armel        Vi IMproved - Common files
ii  vim-runtime                       2:7.4.430-1                    all          Vi IMproved - Runtime files
ii  wget                              1.15-1+b1                      armel        retrieves files from the web
ii  whiptail                          0.52.17-1                      armel        Displays user-friendly dialog boxes from shell scripts
ii  wpasupplicant                     2.2-1                          armel        client support for WPA and WPA2 (IEEE 802.11i)
ii  xkb-data                          2.12-1                         all          X Keyboard Extension (XKB) configuration data
ii  zlib1g:armel                      1:1.2.8.dfsg-2                 armel        compression library - runtime
ii  zlib1g-dev:armel                  1:1.2.8.dfsg-2                 armel        compression library - development
```
