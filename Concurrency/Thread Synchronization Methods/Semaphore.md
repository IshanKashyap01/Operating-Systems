# Semaphore

- It is an *integer variable representing the number of available resources*

- Its value is *decreased* when a lock is *acquired* and *increased* when a lock
is *released*

- *Unlike* locks and conditional variables, *Semaphore* is used when we need to
run *multiple threads* at a time

- In other words, it is used when there are *multiple instances* of a resource

- It allows *multiple* threads to run a *critical section* without running into
a *race condition*

- This is possible because, at any instant, *only one* thread can execute a *critical*
*section*
