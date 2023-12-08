# Conditional Variable

- When a thread is *busy waiting*, it is wasting time on the CPU

- A better way is to *wait* until notified that the lock is lifted

- To implement this approach, a **conditional variable** is used

- It enable threads to go to *sleep inside of critical sections, by releasing*
*their lock at the same time it puts the thread to sleep*

- It has the following two states: **wait** and **signal/notify**

- It makes the threads to *wait* until the needed lock is released

- Once the lock is released, it *notifies* the threads to stop *waiting* so they
can try again
