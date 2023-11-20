# Operations of Processes

## Process Creation

- The **fork()** operation is used to create a new process

- In a Linux system, the first process started is called **Init** with a *PID of 1*

- Every process will have *Init* as its *ultimate parent process* or *root*

## Process Termination

- The operations **exit()** and **kill()** are used to end a process

- When a process *exits* it deallocates all resources and closes all file

- A process may be terminated or *killed* due to:
  - termination by the user
  - lack of resources
  - parent process terminating the child process

- Depending on the OS, termination of a process may result in termination of
child processes as well

## Orphan Processes

- When the parent process terminates leaving a child behind, the child process,
if not terminated as well, becomes an orphan process

- Orphan processes are adopted by *Init* i.e. their *ppid* is changed to 1

- The process is called an orphan because the process initiating it is terminated

## Zombie Process

- When a process is terminated/exits but its *PCB* remains in the *Process table*,
it is called a **zombie process**

- Removal of a child process from  *process table* is the task of its parent process

- If the parent process is in *waiting* while the child process has already exited,
the child process will become a *zombie process*

- Zombie processes creates a problem if the system can have a finite amount of PIDs

- Linux system can have a maximum of 32768 processes
