## Submitting issues on GitHub

Before submitting an issue, please make sure that you have the latest kernel:

    # as root...
    apt-get update
    apt-get upgrade
    apt-get dist-upgrade
    # if a new kernel package was installed
    reboot
    
Also, check the [release notes](https://github.com/ev3dev/ev3dev/tree/master/release-notes)
to make sure it is not a known issue.

In the desription of your issue, be sure to include:

* The image file that you used to flash your SD card (e.g. `ev3dev-wheezy-2014-07-11.img`).
* Your kernel version (output of `uname -rv`)
* The output of `lsusb` if the issue is with an USB device like a WiFi dongle.
* The output of `systemctl status brickman.service -l` if the issue is with the Brick Manager.
* If a screenshot of the EV3 would be helpful, run `fbgrap > <some-name>.png` on the EV3 and include the picture in your comments.
