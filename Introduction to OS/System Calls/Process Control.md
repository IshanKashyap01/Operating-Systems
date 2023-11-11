# Process Control

- Used for creating or terminating a process
- Makes a process wait for a certain time

## System calls in Process Control

These system calls are wrappers around the actual implementation in C.

### Fork()

- It is used to create a new process with a unique process ID

### Exit()

- It is used to terminate a process *properly*

- A process can have memory, files and other chlid processes related to it

- This call will deallocate the memory, close the files and terminate the child
processes

### Wait()

- This call is used to temporarily pause a process
- A parent process can make this call to suspend itself until a child process
finishes i.e. calls Exit() on itself

### Exec()

- This call is used to execute a different code under the same process ID

### Kill()

- This call terminates a process *abruptly* or *cleanly* depending on the signal

- In shell, you have to type the ID of the process followed by the kill command and/or
a signal code

- A hyphen is used before a signal code

- By default, it cleanly terminates a process

#### Signals in Kill()

- 9  : Abruptly kills a process
- 15 : Cleanly terminates a process
- 2  : Terminates a process using a keyboard interrupt
- l  : Lists all the signals with their codes
