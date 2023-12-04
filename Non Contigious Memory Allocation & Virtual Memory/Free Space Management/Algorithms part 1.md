# Algorithms for Free Space Management

- Let's say we have 5 free blocks of memory of sizes **50, 100, 90, 200 and**
**50 KB** respectively

- A process of size **90 KB** is now to be allocated

## Best Fit

- First, it will sort the list of free blocks

- So, the list will look like: *50, 50, 90, 100, 200*

- Then, it will assign P1 to the *smallest block* that can accomodate it

- Hence, P1 will be allocated to the **third block of size 90 KB**

- However, the process will be *slow* due to *sorting and searching*

## Worst Fit

- It will sort the list just like *best fit*

- Then, it will select the *largest block* and carve out the *required size* from
it to assign it to the P1

- Hence, P1 will be allocated to the **fourth block of size 200 KB** creating
a *new* free space block of *110 KB*

- Although, it eliminated searching, it will also be *slow* due to *sorting*

## First Fit

- Instead of sorting the list, it will assign P1 to the **first block of memory**
that can accomodate it

- Hence, P1 will be allocated to the **second block of size 100 KB** leaving behind
a *new* free space block of *10 KB*

- However, it may fill only the first few blocks potentially leading to *fragmentation*

## Next Fit

- The first process will be assigned same as in *first fit* and it will store its
location

- For the next process, it will search for free space right next to that location

- Hence, it will store P1 in the **second block of size 100 KB**

- However, it does not consider optimal fitting of memory blocks leading *increased*
*internal fragmentation*
