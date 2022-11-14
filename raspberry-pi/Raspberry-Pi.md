# Raspberry Pi Devices

<img src="img/raspberry-pi01.jpg" width="600" />

Raspberry Pi models are the most popular [Open Source](https://opensource.com/resources/raspberry-pi) mini-computers in the world and are used by amateur hobbyists and hackers as well as industry professionals in a variety of IoT capacities. They are designed by the [Raspberry Pi Foundation](https://www.raspberrypi.com/documentation/computers/raspberry-pi.html). Two targets are of interest to Tari due to their widespread deployment: 

* **Raspberry Pi 4 B:** This single-board computer has a 64-bit ARM chipset ([arm64](https://wiki.debian.org/Arm64Port) architecture).

* **Raspberry Pi 3 B+:** This single-board computer has a 32-bit ARM hard-float chipset (ARMv7 [armhf](https://wiki.debian.org/ArmHardFloatPort) architecture).

## Raspberry Pi 4 B

<img src="img/raspberry-pi-4-01.jpg" width="600" />

### Documentation

#### Vendor
The Raspberry Pi Foundation publishes a detailed [git repository](https://github.com/raspberrypi/documentation) with most hardware design files as well as a documentation [wiki](https://www.raspberrypi.com/documentation/computers/raspberry-pi.html).

#### Community
The hardware community around Raspberry Pi is huge and very active all over the Web, such as in the  [Raspberry Pi Foundation forums](https://forums.raspberrypi.com/).

### Software

#### Bootloader

The Raspberry Pi 4 [bootloader](https://pimylifeup.com/raspberry-pi-bootloader/) is loaded via EEPROM.

#### Operating System

Raspberry Pi models ship with a [Debian GNU/Linux](https://debian.org) derivative called [Raspbian](https://raspbian.org) via the [NOOBS installer](https://www.raspberrypi.com/software/). Instructions for flashing and updating the OS [are available here](https://thepi.io/how-to-install-noobs-on-the-raspberry-pi/).

#### Connecting to the Device

The system starts the Raspbian [LXDE](https://lxde.org) desktop environment when it boots. The easiest way to access it is [connecting to a display](https://www.raspberrypi.com/documentation/computers/getting-started.html#connecting-a-display) or via [the network](https://www.raspberrypi.com/documentation/computers/remote-access.html#introduction-to-remote-access).

#### Tari Testing &amp; Compatibility

The Tari suite `arm64` builds for [Ubuntu](https://ubuntu.com) will run on the Raspberry Pi 4 B with Raspbian.

Some Debian dependencies must be installed:
* [Tor](https://www.linuxcapable.com/how-to-install-tor-browser-on-debian-11-bullseye/) must be installed and the [control port 9051](https://manpages.debian.org/testing/tor/torrc.5.en.html) will need to be open and configured in `/etc/tor/torrc`.
* _NOTE_ The Tari suite `start_all` script requires the [GNOME](https://www.gnome.org) desktop environment. This DE is not recommended on this device so the script should be ignored or modified for Raspbian.

Instructions: 
* Download the `arm64` build of `tari_suite` from the [Tari downloads page](https://www.tari.com/downloads/).
* Verify the SHA256 checksum for the file.
* Copy the ZIP archive to the device and extract the files with `unzip`.
* Change the permissions on the Tari binaries to be executable.
* Run the Tari binaries via the CLI.

Additional installation instructions are available in the [Tari project repositories](https://github.com/tari-project/tari/blob/development/README.md).

## Raspberry Pi 3 B+

<img src="img/raspberry-pi-3b-01.jpg" width="600" />

### Documentation

#### Vendor
The Raspberry Pi Foundation publishes a detailed [git repository](https://github.com/raspberrypi/documentation) with most hardware design files as well as a documentation [wiki](https://www.raspberrypi.com/documentation/computers/raspberry-pi.html).

#### Community
The hardware community around Raspberry Pi is huge and very active all over the Web, such as in the  [Raspberry Pi Foundation forums](https://forums.raspberrypi.com/).

### Software

#### Bootloader

The Raspberry Pi 3 [bootloader](https://pimylifeup.com/raspberry-pi-bootloader/) is loaded via a `bootcode.bin` file on the boot filesystem (microSD card).

#### Operating System

Raspberry Pi models ship with a [Debian GNU/Linux](https://debian.org) derivative called [Raspbian](https://raspbian.org) via the [NOOBS installer](https://www.raspberrypi.com/software/). Instructions for flashing and updating the OS [are available here](https://thepi.io/how-to-install-noobs-on-the-raspberry-pi/).

#### Connecting to the Device

The system starts the Raspbian [LXDE](https://lxde.org) desktop environment when it boots. The easiest way to access it is [connecting to a display](https://www.raspberrypi.com/documentation/computers/getting-started.html#connecting-a-display) or via [the network](https://www.raspberrypi.com/documentation/computers/remote-access.html#introduction-to-remote-access).

#### Tari Testing &amp; Compatibility

The Tari project does not provide builds for the `armhf` architecture, so the Tari suite must be compiled from source on the Raspberry Pi 3.

Instructions for compiling from source are available in the [Tari project repositories](https://github.com/tari-project/tari/blob/development/README.md).

Some Debian dependencies also must to be installed: 
* [Tor](https://www.linuxcapable.com/how-to-install-tor-browser-on-debian-11-bullseye/) must be installed and the [control port 9051](https://manpages.debian.org/testing/tor/torrc.5.en.html) will need to be open and configured in `/etc/tor/torrc`.
* [unzip](https://packages.debian.org/stretch/unzip) is required to extract the Tari binaries.
* _NOTE_ The Tari suite `start_all` script requires the [GNOME](https://www.gnome.org) desktop environment. This DE is not recommended on this device so the script should be ignored or modified for Raspbian.

