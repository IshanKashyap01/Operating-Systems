# File System

The file system keeps track of all the files and directories in the system by
using the **inode**

## Contents of Inode

- **Inode number** is the unique id assigned by OS to each file and directory

- **Mode information** describes whether it is a file or a directory which is
generally *755* for a *directory* and *644* for a *file*

- **Number of links** or *shortcuts* to the file or directory

- **UID of the owner**, which is the *user ID* of the owner

- **GID of the owner** i.e. the *group ID* of the group with the ownership of
the file

- **Size** of the file/directory

- **Number of blocks** the file/directory is using on the disk

- **Last modified** time or the *mtime*

- **Last accessed** time or the *atime*

- **Last changed** time or the *ctime*
