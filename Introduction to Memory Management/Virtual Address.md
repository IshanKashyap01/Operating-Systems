# Virtual Address Translation & Protection

- The mapping of a process' address space from virtual to physical memory is known
as **address translation**

- It is done by both *OS and underlining h/w* via the **base and bound** technique

## Base and Bound Technique

- The underlining h/w will have two *registers* known as **base** and **bound**

- The *base* register is used to store the *starting* physical address of a process

- To get the address of next instruction, the following formula is used:

    **Physical address = base + virtual address**

- The *bound* register is used to store the *maximum size* of the address space

- The *base* register is used for *translation* of data whereas, the *bound* register
is used for the *protection* of data

- These *base and bound registers* present on the hardware are also known as
**Memory Management Unit**

- An address is valid **only** if it lies b/w the *base* and the *base + bound*
values of the process
