# Introduction to Memory Management

## Memory Management in Early Days

- Suppose the main memory is of size 128 KB and OS takes the first 64 KB
- The remaining 64 KB will be free to use for processes
- Now, OS will assign this *entire memory* to a **single process** until its completion
- Hence, other processes will have to remain in secondary memory and wait until
they are loaded into the main memory
- The **drawback** with this approach is *low efficiency* and **multiprogramming**
was introduced to solve it

## Multiprogramming with Time Sharing

- **Time sharing** was used with the help of *disk/secondary memory*
- A fixed amount of time was granted to each process to run until it gets replaced
- The whole main memory was still granted to the running process while other
processes remained in the disk
- To switch b/w processes, OS *state saved* current process to the disk and performed
*state restore* on the next process
- The **drawback** with this approach is that secondary memory is *too slow*

## Solution to Time Sharing using Disk

- To make time sharing *more efficient*, the state and other info of processes
were stored in the main memory itself
- Now, instead of giving the *entire memory* to a single process only a *small portion*
was granted to a process
- This way *multiple processes* could be stored in the memory
- The new **problem** that arrived with this approach was *how to isolate the*
*processes* from each other
- This problem was solved by the **virtualisation of memory**
