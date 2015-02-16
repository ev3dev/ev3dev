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
* If you are using a library (ev3dev-lang, python-ev3, ev3dev-c, etc.) please state which library. Most, if not all, of these have their own issues tracker. You may have better luck posting there instead.
* If the issue is with detection of a sensor or motor: unplug and plug in the device and include the output of `dmsg | tail`/
* If the issue is with an USB device like a WiFi dongle: include the output of `lsusb`.
* If the issue is with the Brick Manager (brickman): include the output of `systemctl status brickman.service -l`.
* If a screenshot of the EV3 would be helpful, run `fbgrab <some-name>.png` on the EV3 and include the picture in your comments.

If you are posting logs that are more than 5-10 lines long, please use http://pastebin.com or https://gist.github.com or something similar instead of posting long logs in comments.
