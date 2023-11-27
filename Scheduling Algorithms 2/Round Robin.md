# Round Robin (RR)

- It is the preemptive version of FCFS
- It has a **time quantum**, which means every process is allowed a set amount
of time before it is preempted
- It works in a cyclic fashion i.e. once the last process has ran for the time
quantum, it will assign the first process back to the CPU.
- If a process ends b/w a cycle, it will restart the cycle
- This algorithms increases **response time** and eliminates the *convoy effect*
