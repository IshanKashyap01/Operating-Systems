# Mulitlevel Queue Scheduling (MLQ Scheduling)

- Processes are categorised into three categories based on priority:
    1. **System** processes
    2. **Interactive** processes (*foreground* processes)
    3. **Batch** processes (non-interactive or *background* processes)

- System processes have the highest whereas batch processes have the least priority

- This algorithm bifurcates the ready queue into multiple queues based on priority
i.e. the algorithm will allocate CPU based on the priority of the queue

- Each queue can have its own scheduling algorithm

## Fixed Priority Preemptive Scheduling

- As long as a higher priority queue contains processes, processes in the lower
queues will have to wait

- This can *starve* the processes in lower queues

- This algorithm allows preemption i.e. if a higher priority queue gets a process,
then the current process will be preempted and the higher queue will get the CPU

## Scheduling Based on Time Slice

- Here, the algorithm decides a time quantum and each process in a queue will run
only for that time

- This time quantum can differ for different queues

- For instance, Q1 can get 50%, Q2 can get 30% and Q3 can get 20% of the time
quantum
