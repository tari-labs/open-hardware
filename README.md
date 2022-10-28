# Running Tari on Open Hardware platforms

<img src="img/open-hardware-devices01.jpg" width="600" />

[Tari](https://tari.com) is a digital assets focused blockchain protocol that is built in Rust, private by default, and is being architected as a merge-mined sidechain with [Monero](https://monero.org). In a world without default privacy, businesses cannot operate, our personal preferences and histories are sold to the highest bidder, and we lose the ability to conduct our lives in the manner we choose. The Tari community fundamentally believes that privacy-enhancing software should be pervasive and available to all.

The Tari project releases its code as Free and Open Source Software (FOSS) and is designing a codebase that will empower developers of any skill level to quickly build useful applications that leverage the Tari network. The best way to get started is to start running a Tari node. A Tari node is the basic building block of the Tari blockchain and network. Nodes perform the critical functions of maintaining the ledger. Without nodes, there is no network.

This repository is one aspect of the Tari project's dedication to FOSS and Open Hardware platforms. We will provide documentation and guidance here that will be useful for users who intend to run Tari on Open Hardware. Additionally, we will post updates here about Tari proof-of-concepts, testing, and compatibility with hardware such as single-board computers.

Tari currently runs on a variety of popular platforms such as [Raspberry Pi](https://www.raspberrypi.com) and the [Open Source Hardware](https://www.oshwa.org/definition/) (OSHW) approved [Beaglebone](https://beagleboard.org/bone). It also runs on hardware certified by the Free Software Foundation (FSF) as [Respects Your Freedom](https://ryf.fsf.org) (RYF).

## Hardware 
_These platforms are listed in order of known stability running Tari._

* [RYF Thinkpad T500](fsf-ryf/Thinkpad-T500.md) (x86_64)
* [Raspberry Pi 4](raspberry-pi/Raspberry-Pi-4.md) (arm64)
* [BeagleBone AI-64](beaglebone/BeagleBone-AI.md) (arm64)

_We are currently planning to run Tari on these platforms._
* [Raspberry Pi 3](raspberry-pi/Raspberry-Pi-3.md) (armhf)
* [BeagleBone AI](beaglebone/BeagleBone-AI.md) (armhf)
* [Precursor](risc-v/Precursor.md) (risc64)
* [PINE64 Star64](risc-v/Star64.md) (risc64)

<img src="img/tari-base-node.png" width="300" />

## Licensing

These materials are ethical Free and Open Source Software (FOSS). Any and all original work contained in this repository is copyright &cop; 2022 Tari Labs and released under the BSD 3-Clause License. See [LICENSE](LICENSE) for more information.
