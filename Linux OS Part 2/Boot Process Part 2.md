# Boot Process Part 2

## Kernel

- It mounts the *root file system* and execute the *init* process present at
**/sbin/init**

- It will also mount a the **initial RAM disk (initrd)** which will have information
about *device drivers*

- The *initrd* serves as a temporary storage until the *root file system* gets
loaded

## Init

It first starts all the background processes followed by the *run level*

## Run Level

- The information for *run level* is stored in the **/etc/inittab** file

- The run level starts from *level 0 to level 6* where:
    0. Halt mode
    1. Single user
    2. Multiuser mode w/o NFS
    3. Multiuser mode w/ NFS
    4. Not used
    5. GUI mode
    6. Reboot

- The corresponding files for run level are stored under **/etc/rc*.d/** where
the asterisk represents the level number

- In some systems, the file may be present under **/etc/rc.d/rc*.d**

- Once, the run level is executed, user will be prompted for login and system
will be ready for use

- The **runlevel** command can be used to check the current run level
