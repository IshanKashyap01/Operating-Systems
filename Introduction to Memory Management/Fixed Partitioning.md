# Problems with Fixed Partitioning

## Internal Fragmentation

- Suppose a process is alloted a slot of 6 MB but it only needs 3 MB

- The remaining 3 MB cannot be utilised by some other process and is wasted

- This is known as **internal fragmentation**

## Degree of Multiprogramming

- Due to a fixed number of slots, the amount of processes in the ready queue
cannot exceed the total number of slots

- Hence, the degree of multiprogramming is **fixed**

## Size of Processes

If a process needs more size than the largest partition, it will **never** be assigned

## External Fragmentation

- Suppose there are ten partitions for processes each occupied by some process

- Now, let's say some of them have internal fragmentation leading to a total of
20 MB of free memory

- Now, a new process that needs even 1 MB of space cannot be assigned as the unused
space is not contigious
