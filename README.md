# About this repository

This repository is the Chromium OS board overlay for the [Asus Tinkerboard single board computer](https://www.asus.com/us/Single-Board-Computer/Tinker-Board/).

The code and document in this repository is the result of work by Matt and previous works by the people of the FydeOS team. FydeOS previously worked on this overlay internally and released a few disk images to the public, but later opened this to the public so people can build the OS by themselves and improve it.


# How to build it

Please refer to the README in the [Chromium OS for Raspberry Pi](https://github.com/FydeOS/chromium_os_for_raspberry_pi) repo for how to setup and build Chromium OS. The instructions there are not completely relevant for Tinker Board, but I managed to build this on Ubuntu 14.04 LTS (only) by running 'mkdir ~/project' and 'sudo mv ~/project /project' (doing it exactly as written doesn't work, and running mkdir as root created permission issues later).  
Reminder 1: Edit `~/trunk/src/third_party/chromiumos-overlay/eclass/cros-board.eclass` and add `tinker` to the list.
Reminder 2: There are problems with some of the licenses in the linux-firmware folder. Just write empty files for now to progress.
