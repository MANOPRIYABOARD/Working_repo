mkudoobuntu

This script creates SD-card images for seco boards. It supports both desktop and headless images. The created images are as small as possible and expanded to the whole card size during the first boot.

Usage

To debootstrap a new unnamed image, use:

sudo ./mkudoobuntu.sh <board> <flavour>
Branded-release images can be generated with:

sudo RELEASE="2.0 Beta6" ./mkudoobuntu.sh <board> <flavour>
To edit a previously debootstrapped rootfs, use:

sudo ./mkudoobuntu.sh <board> <operation>
<board> can be: udoo-qdl, udoo-neo.

<operation> can be:

install: Install a deb in rootfs from repos
remove: Remove a deb from rootfs
list: List installed pkg in rootfs
reimage: Make a new image from a modified rootfs
shell: Open an interactive shell in a rootfs
Prerequisites

This script has been tested on Ubuntu 16.10, 16.04, 15.10, 15.04 and 14.04. It may work on other Debian-like system.

Supported boards

UDOO Quad
UDOO Dual
UDOO Neo (Basic, Extended, Full)
Misc sources

Original work: https://github.com/igorpecovnik/lib

U-Boot: https://github.com/MathanrajMurugan/Working_repo/tree/master/u-boot-2015-04-secoboards-imx6sx-rel

Kernel: https://github.com/MathanrajMurugan/Working_repo/tree/master/linux-4-1-15-secoboards-imx6sx-rel
