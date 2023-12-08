# Locking

- It is used when multiple instructions needs to be atomic

- It prevents multiple threads to access a resource simultaneously

- A lock has two states **locked** and **available**

- If the lock is in *available* state, any thread can access it

- However, the moment a thread accesses it, it changes its state to *locked*,
blocking everyone else from using it

- Once the thread finishes using the resources, it then *unlocks* the resource,
making it available for other threads

- If the active thread needs a locked resource, it will constantly check for it
to be unlocked before proceeding its execution

- This is called as **busy waiting**, **busy looping** or **spinning**

## Issues with Locking

### Contention

When a lock needed by the active thread is held by a wating thread resulting in
*busy waiting*

### Deadlock

- Suppose, there are resources *r1* and *r2* needed by threads *t1* and *t2* respectively

- Now, let's say *r1* is locked by *t2* and *r2* is locked by *t1*

- In this scenario, both the threads have locked each other's resources resulting
in a perpetual lock

### Debugging

Locks increases complexity of code making debugging difficult

### Starvation

When a low priority thread acquires a lock needed by a high priority thread
