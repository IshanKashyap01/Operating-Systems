# Advantages of Dynamic Partitioning over Fixed Partitioning

- As partition sizes are granted wrt the process, there is no *internal fragmentation*

- Degree of multiprogramming is *variable* and generally *higher*

- Any size of process can be assigned as long as enough free and contigious memory
is available

## Example of External Fragmentation in Dynamic Partitioning

- Suppose there are three contigious processes in the main memory where:
  - First process is taking up 20% memory
  - Second process is taking up 50% memory
  - Third process is taking up 30% memory

- Now, let's say the first and third processes frees up and a new process comes
up that requires 40% memory

- Although, there is 50% free space the process cannot be accomodated as it is not
contigious
