# Files and Directories

- The OS abstracts the physical properties of storage devices into **files** and
**directories**

- A *file* is the smallest logical unit of data from a user's perspective

- When a *file* is created, the OS assignes it a unique **inode number** also known
as a **file serial number**

- Similarly, a *directory* is also assigned an *inode number*

- The first few bits of a file denotes the *file format* and are called the
**magic number**

## Open File Table

- It contains a list of all the *open files* along with:
  - File Pointer
  - File-open Count
  - Disk Location
  - Access Rights

- The **file pointer** points to the current location in the file where the *next*
*read-write* operation will take place

- The **file-open count** represents the number of processes accessing the file
at the moment

## Locks on Files

- A **shared lock** is used for *read-only* operations

- An **exclusive lock** is used for *read-write* operations

- An **advisory lock** is an *informational lock* that gives warning to processes
that the file is accessed by other processes

- A **mandatory lock** is an *enforced lock* that denies access requests if the
file is currently in use

- *Linux* uses an *advisory lock* whereas *Windows* uses a *mandatory lock*
