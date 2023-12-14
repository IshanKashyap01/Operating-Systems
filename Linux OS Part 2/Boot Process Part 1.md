# Boot Process Part 1

## Basic Input Output System (BIOS)

- When the system is powered on, the BIOS will execute and do h/w verification

- If everything is fine, it will load the MBR

- It is part of the h/w and has nothing to do with the OS

## Master Boot Record (MBR)

- It is present at the first sector of the *bootable disk* and will generally be
of 512 B in size and loads the GRUB

- It has information related to the *boot loader* and *disk partitioning*

## Grand Unified Bootloader (GRUB)

- It loads the Kernel and its configuration is under **/boot/grub/grub.cfg**

- The file contains info about boot disk, splashscreen, root partition etc.

- If we have multiple Kernels, it will display a splashscreen to ask which one
to load

- By default, the latest Kernel is loaded, however, the splashscreen will remain
until we either choose a Kernel or press enter
