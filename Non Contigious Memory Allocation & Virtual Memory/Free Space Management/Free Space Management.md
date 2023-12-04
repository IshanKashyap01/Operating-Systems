# Free Space Management

- Suppose we have an empty RAM with just the OS loaded and the remaining free
space is 12 KB

- This free space will look like a **chunk of 12 KB**

- Let's say, a process P1 comes requesting a size of *2 KB*, the process will be
allocated and the free space will look like a **chunk of 10 KB**

- Now, a process P2 with *8 KB* is allocated adjacent to P1

- The free space will now look like a **chunk of 2 KB**

- Now, a process P3 with *2 KB* is allocated so there is no free space

- Now, let's say, P3 is terminated. The free space will look like a **chunk of 2**
**KB**

- Now, P1 terminates resulting in **two separate chunks of 2 KB each**

- After P2 terminates, there will be **three adjacent chunks of 2, 8 and 2 KB**

- The allocator will check adjacency of different chunks, every time there are
two or more free chunks and merge the adjacent ones

- So, in this case, the allocator will merge the chunks into a **chunk of 12 KB**
