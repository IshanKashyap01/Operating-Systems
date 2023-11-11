# Types of Kernel

## Monolithic Kernel

This type of kernel contains all the OS related modules inside the kernel as
single piece of code.  
Example: Linux and Unix

### Structure

#### User space

- Applications

#### Kernel

- Process manager
- Memory manager
- File manager
- I/O manager

### Pros

1. Communication b/w modules is quite fast as everything is in the same place

### Cons

1. Takes a lot of memory
2. Failure in one module will crash the entire OS

## Micro Kernel

- In this, only the major functionality is present in the kernel while the rest is
in user space.  
- The OS keeps switching b/w user space and kernel to use the different
components  
- This switch is done by using Interprocess Communication (IPC) present in the kernel
- Example: L4Linux and SymbianOS

### Structure

#### User space

- Applications
- File manager
- Device drivers

#### Kernel

- Memory manager
- Process manager

### Pros

- Takes less space
- Modules are separated so if one crashes, the others will keep working

### Cons

- OS has to switch b/w the components creating a lot of overhead
- It is not as portable as it is designed for special type of hardware

## Hybrid Kernel

This type of Kernel solves the problems faced in the other types while retaining
their advantages.  
Example: Windows 7, 10 and MacOS

### Structure

#### User Space

- Applications
- File manager

#### Kernel

- Device driver
- Memory manager
- Process manager

### Pros

- Consumes less space than monolithic kernel
- Lower number of switches than Micro kernel resulting in less overhead
- It is more reliable than monolicthic kernel

&nbsp;

**Note**: *Nano and Exo kernels are not discussed here*
