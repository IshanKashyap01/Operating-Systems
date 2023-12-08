# Process vs Thread

- A *process* can have *multiple threads* but a *thread* can belong to *only one*
process

- All the threads of a process lies *within the address space* of the process

- In a single thread process, the address space has a block of program code,
stack and heap

- A process with multiple threads, have *multiple stacks, one for each thread*

- However, they still share the *same program code and heap memory*

- Similar to a process, threads also undergoes *context switch*, in which case,
its properties are stored in a **Thread Control Block**

- Basically, threads are treated as **mini processes** by the OS as they have their
own *control block* and *scheduling algorithms*
