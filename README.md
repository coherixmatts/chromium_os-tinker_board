# About this repository

This repository is the Chromium OS board overlay for the [Asus Tinkerboard single board computer](https://www.asus.com/us/Single-Board-Computer/Tinker-Board/).

The code and document in this repository is the result of work by Matt and previous works by the people of the FydeOS team. FydeOS previously worked on this overlay internally and released a few disk images to the public, but later opened this to the public so people can build the OS by themselves and improve it.


# How to build it

Please refer to the README in the [Chromium OS for Raspberry Pi](https://github.com/FydeOS/chromium_os_for_raspberry_pi) repo for how to setup and build Chromium OS. The instructions there are not completely relevant for Tinker Board, but I managed to build this on Ubuntu 16.04 LTS installing to ~/project instead of /project (due to errors with permissions doing it exactly as written).  
Reminder 1: Edit `~/trunk/src/third_party/chromiumos-overlay/eclass/cros-board.eclass` and add `tinker` to the list. 
Reminder 2: Build packages in chroot with --nousepkg
