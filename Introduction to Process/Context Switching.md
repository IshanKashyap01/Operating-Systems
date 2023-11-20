# Context Switching

- The process of changing the running process is called context switching

- The OS uses information stored in the PCB to correctly start/restart a process

- The OS performs a *state save* on the current process and a *state restore* on
the next process to be started/resumed

## When does the OS performs a Context Switch

- When the running process enters a waiting state, OS, via context switch, changes
to another process

- When a process is terminated, OS uses context switch to move to the next process
