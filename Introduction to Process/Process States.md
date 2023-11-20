# Process States

## New

- When OS is about to pick a program and convert it into a process
- These processes are in secondary memory

## Ready

- When a process is picked by OS and stored in main memory  

- A *running* process can change to this state depending on priority or if it runs
out of time

## Running

- When a process is under execution  

- OS picks processes from *ready* state to run them one by one

## Terminate

When a process is completed without errors and exits

## Wait/Block

- When a running process is waiting for user input or an I/O operation to finish  

- Here, the process is not using the CPU so OS will assign another process for
execution

- Once the I/O is finished, it moves to *ready* state

## Suspend/Ready

- When a process is in *ready* state but there is no free memory and a higher priority
process in the queue, and OS moves this process to secondary memory to free space

- Once there's enough memory, OS will move the process back to *ready* state

## Suspend/Wait

- When a process is in *wait/block* state but there is no free memory and a higher
priority process in the queue, and OS moves this process to secondary memory to
free space  

- When the I/O is complete but there is still not enough memory, this process will
move to *suspend/ready* state otherwise, it will revert to the *wait/block* state
