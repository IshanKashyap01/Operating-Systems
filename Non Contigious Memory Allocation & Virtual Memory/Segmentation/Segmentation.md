# Segmentation

- It is a *non contigious memory allocation method*

- The physical memory is divided into *continuous* blocks of memory of different
sizes known as **segments**

- It uses **three pairs of base and bound registers** as a process is divided
into *three blocks* (each assigned to a different segment):
    1. Code
    2. Stack
    3. Heap

- Obviously, the virtual address of the process remains a single continuous block
