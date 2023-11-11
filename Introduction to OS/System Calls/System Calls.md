# System Calls

- As we know, OS is divided into two parts and the system switches b/w them whenever
it needs a component from either of them

- This switch is done by making a "System call" to the OS/Kernel

- Whenever an app or a user needs to interact with the hardware/OS it makes a
system call to the OS

## Types of System Calls

- Process control
- File management
- Device management
- Information management
- Communication

## Device Management

- This category of system calls are used to interact with the h/w

- Certain OSs like Unix provide the same calls for this as file management
like **open()** and **read()**

- It also has calls like **attach()** to connect and **detach()** to disconnect
a device

### Information Management

- The OS keeps track of information such as date & time, free space on disk,
allocated and free memory in RAM, OS version, process IDs etc.

- It uses calls such as getpid() and getppid() to get process or parent process
IDs respectively

### Communication

This contains system calls such as pipe(), shm-open() and mmap()
