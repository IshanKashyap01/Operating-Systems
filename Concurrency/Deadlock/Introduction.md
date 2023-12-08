# Deadlock

It is a *bug* where a set of processes blocks each other and cannot proceed further

## Conditions for Deadlock

### Mutual Exclusion (MUTEX)

- Threads acquire exclusive control over a resource, preventing others from using
it until released

- If the thread is unable to release the resource for some reason, other processes
depending on the resource cannot finish

### Hold & Wait

A thread is currently holding at least one resource and requesting additional
resources which are being held by other processes

### No Preemption

- A thread needs resources held by some inactive threads and is therefore, unable
to proceed further

- However, due to no preemption, the process will continue waiting forever

### Circular Waiting

A chain of threads all waiting for each other to release some resources so they
can proceed
