# Key Terms in Concurrency

## Critical Section

A piece of code that performs operations on shared resources, usually a shared
variable or data structure.

## Race Condition

- It occurs when multiple threads *simultaneously* runs a critical section

- This can lead to unpredictable and undesired results

## Indeterminate Program

- A program with *one or more race conditions* and hence, with an unpredictable
output

- Its output depends on the order in which the threads runs as well as where they
were preempted which changes every time the process is repeated

## Mutual Exclusion

It states that *only one* thread enters and executes a *critical section* at a
time hence, preventing *race conditions*
