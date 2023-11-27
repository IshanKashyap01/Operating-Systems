# Priority Scheduling

- In this algorithm, processes are assgined a priority
- Based on the priority, a process will be assigned to the CPU
- This algorithm can create a *convoy effect*

## Non Preemptive Priority Scheduling (NPPS)

In this algorithm, if a higher priority process enters after a lower priority
process is already dispatched to the CPU, it will keep the higher priority process
in waiting

## Preemptive Priority Scheduling (PPS)

In this algorithm, while a process is running on the CPU, a higher priority process
enters the ready queue, it will preempt the current process to run the higher
priority process
