# Disk Scheduling Algorithms

## First Come First Serve (FCFS)

- Requests are served in the same order they they were requested

- A benifit of this algorithm is that there is *no starvation* as every request
is served in the order it appears

## Shortest Seek Time First (SSTF)

- The request *closest* to the current position of the *read-write head* is served
first

- However, if a request is far away from the current position, it can lead to *starvation*

## SCAN (Elevator Algorithm)

- The *read-write head* moves in one direction until it *reaches the end*, then starts
moving in the *reverse direction*

- It is simple, easy to implement, more efficient than *FCFS* and *free of starvation*

- However, cannot change direction until it reaches *either ends of the disk*

## C-SCAN (Circular Scan Algorithm)

- Similar to *SCAN*, it will move in *only one direction* however, upon reaching
the end, it will *move back to the start* and begin again

- In addition to *SCAN's* disadvantage, it wastes even more time getting back in
position

## Look Algorithm

It works *just like SCAN* except it switches direction when it reaches the *last*
*request* in the direction rather than the *end of disk*

## C-Look Algorithm

It works *just like CSCAN* except it *returns to the start* when it reaches the
*last request* in the direction of its movement
