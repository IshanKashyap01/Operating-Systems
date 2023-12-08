# How to Prevent Deadlock

## Mutual Exclusion (MUTEX)

- Do not use locks for *read-only* resources
- Use locks only for *non-shareable* resources

## Circular Wait

Define a linear ordering of resources such that a thread cannot acquire a lock
if it does not acquire the ones preceeding it

## No Preempting

1. To acquire a new resource, release the old one and try to acquire both simultaneously
    - This may lead to different threads trying to acquire a lock simultaneously
    - This collision, called **livelock** can be prevented by adding delays to
    each process

2. Make the waiting/blocked threads release the locks needed by the active thread

## Hold & Wait

1. Enforce that a process acquires all the locks it needs at once. However, it
leads to wastage of resources

2. Release the already acquired resource and try to reacquire it when all the needed
locks are available
