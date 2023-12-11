# File System in Linux

    $ ls /
    ishan@Operating Systems$ ls /
    bin   dev  home  lib    lib64   lost+found  mnt  proc  run   snap  sys  usr
    boot  etc  init  lib32  libx32  media       opt  root  sbin  srv   tmp  var

    $ du /boot
    4       /boot

- In linux, the system has multiple partition, each with its own *file system*
and everything is a file

- **df** command is used to check the usage of these partitions

- **-h** flag can be added to get output in a human readable format

- **du** command returns the usage of of the given directory

- In linux, all files are stored under the parent directory **/**

- Each directory under **/** has a special purpose

## Directories under /

- **/bin/** essential user command binary files

- **/boot/** files required for booting

- **/dev/** device files

- **/etc/** system config

- **/home/** user's home directory

- **/lib/** shared libraries for *bin* and *sbin* directories

- **/media/** for mounting removable drives

- **/mnt/** for mounting the temporary file system

- **/opt/** add-on application

- **/sbin/** system binary files

- **/srv/** data from different services like ftp servers

- **/temp/** temporary files

- **/usr/** user application and utilities

- **/proc/** process information
