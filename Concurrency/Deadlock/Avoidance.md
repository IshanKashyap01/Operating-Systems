# Deadlock Avoidance

- It is done by scheduling the threads such that a deadlock is not possible

- Such a case is called **safe state**, whereas a scheduling where a deadlock
can occur, is called an **unsafe state**

- It can be achieved by knowing all the resources a thread will need in advance

- Only the threads that can complete their execution with the available resources
are scheduled to the CPU

- If a thread requires more resources, it will wait until the needed resources
are available

## Banker's Algorithm or Deadlock Detection Algorithm

- It is a resource allocation and deadlock avoidance algorithm that simulates the
allocation process to find a *safe state*

- It keeps a track of the amount of resources already *allocated*, *available*,
and the *maximum* amount of resources needed, by each thread

- It calculates the *remaining* needed resources for each thread to find a sequence
of execution where there's *always at least one thread* that can finish execution
