# Free Software Foundation "Respects Your Freedom" Devices

Tari believes in testing on hardware certified by the [Free Software Foundation](https://www.fsf.org) (FSF) as [Respects Your Freedom](https://ryf.fsf.org) (RYF). The RYF certification program encourages the creation and sale of hardware that accomplishes as much as possible to respect freedom, privacy, and control over devices. This means [Free Software](https://en.wikipedia.org/wiki/Free_software) from the BIOS on up.

## Thinkpad T500

<img src="img/libreboot-thinkpad-t500-01.jpg" width="400" />

Many Lenovo Thinkpad models (often branded IBM) released over the past two decades are certified RYF due to their lack of proprietary firmware requirements and the ability to flash the BIOS with the Free Software replacement [LibreBoot](https://libreboot.org/). Tari is currently testing on the Thinkpad T500 model, but the information below largely applies to all Thinkpad models listed on [this wiki](https://ryf.fsf.org/index.php/categories/laptops).

### Documentation

Information about RYF Thinkpad models is [published by the FSF](https://ryf.fsf.org/index.php/categories/laptops).

### Software

#### Bootloader

The BIOS is [LibreBoot](https://libreboot.org/) on models purchased from [RYF-approved vendors](https://ryf.fsf.org/index.php/categories/laptops) such as Technoethical, Taurinus, and Vikings. Otherwise the BIOS must be [flashed manually](https://libreboot.org/docs/hardware/t500.html).

#### Operating System

Models purchased from [RYF-approved vendors](https://ryf.fsf.org/index.php/categories/laptops) ship with an [Ubuntu](https://ubuntu.com) derivative called [Trisquel GNU/Linux](https://trisquel.info/)

<img src="img/trisquel01.jpg" width="800" />

#### Connecting to the Device

The system starts the Trisquel [LXDE](https://lxde.org) desktop environment when it boots.

#### Tari Testing &amp; Compatibility

The Tari suite `x86_64` builds for [Ubuntu](https://ubuntu.com) will run on the Thinkpad T500 with Trisquel.

Some Ubuntu dependencies must be installed:
* [Tor](https://www.linuxcapable.com/how-to-install-tor-browser-on-debian-11-bullseye/) must be installed and the [control port 9051](https://manpages.debian.org/testing/tor/torrc.5.en.html) will need to be open and configured in `/etc/tor/torrc`.
* _NOTE_ The Tari suite `start_all` script requires the [GNOME](https://www.gnome.org) desktop environment. This DE is not recommended on this device so the script should be ignored or modified for Trisquel.

Instructions: 
* Download the `x86_64` build of `tari_suite` from the [Tari downloads page](https://www.tari.com/downloads/).
* Verify the SHA256 checksum for the file.
* Copy the ZIP archive to the device and extract the files with `unzip`.
* Change the permissions on the Tari binaries to be executable.
* Run the Tari binaries via the CLI.

<img src="img/trisquel-tari01.jpg" width="800" />


