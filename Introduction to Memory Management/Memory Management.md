# Memory Allocation and Management Techniques

- Memory allocation can be either **contiguous** or **non contiguous**

- Management techniques depend on the type of allocation

- For contiguous allocation, we have two memory management techniques:
    1. Fixed partitioning
    2. Dynamic partitioning

## Fixed Partitioning

- It is a method used by OS to allocate memory to processes in the RAM

- OS divides the memory into equal or different but fixed sized slots and each
of them can only be used by a *single process*

- These slots are continuous blocks of memory and none of them overlap with each
other

- The *first slot* is occupied by the OS and the rest are used by processes

## Dynamic Partitioning

- It is a method used by OS to allocate memory to processes in the RAM

- The OS creates a slot in the RAM for itself and the rest is free memory

- The OS dynamically assigns only the required amount of memory to the processes

## Problem with contiguous Memory Allocation

- Any free/unused non-contiguous space in the main memory will be wasted as only
a contiguous block of memory can be assigned to a process

- This is known as **external fragmentation**
