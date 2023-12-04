# Algorithms for Free Space Management (cont.)

## Segregated List

- Let's say, we know how much memory an app requests

- It will reserve that size of memory chunk for that app

## Buddy Allocation

- Let's say, our memory can be represented as a **power of 2**

- It will *break the memory into two halfs* until it gets the smallest chunk that
can fit the process

- So, if we have *64 KB* of memory, it will divide it into two halves of *32 KB*,
then the 32 to *16 KB* and so on

- Once it reaches a chunk that *cannot be assigned*, it goes back one step and
assigns the memory to the process

- Let's say it gets a process of size 6 KB, it will assign it into an 8 KB block

- Once this 8 KB block is freed, if its adjacent half is also free, it will **merge**
the two

- However, it can cause **internal fragmentation** as *2 KB* of memory was wasted
here
