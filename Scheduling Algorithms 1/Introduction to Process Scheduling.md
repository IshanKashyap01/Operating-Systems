# Process Scheduling

The objective of process scheduling is to select the most desirable process
and dispatch it to the CPU

## Reasons for a process to be selected

1. To provide maximum CPU utilization
2. Minimum **Turn Around Time**
    - TAT is the time it took for a process from the moment it enters the ready
    queue to its termination
3. Minimum **Wait Time**
    - WT is the time a process remains in the ready queue
4. Minimum **Response Time**
    - Time taken by a process from the moment it enters the ready queue to the
    first time it runs in the CPU

**Burst Time** is the time it takes for a process to complete. It includes *CPU time*
i.e. the time it takes to run on the CPU and *I/O time* i.e. the time it takes
finish I/O operations
