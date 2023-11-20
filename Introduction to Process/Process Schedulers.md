# Job Schedulers

## Degree of Multiprogramming

It is defined as the number of processes in main memory

## Long Term Scheduler

- It is also known as Job scheduler
- It is responsible for moving processes from *job queue* to *ready queue*
- It continues to moves processes as long as there is memory is ready queue
- It picks a mix of I/O and CPU intensive processes to maintain a *high degree* of
multiprogramming

## Short Term Scheduler

- It is also known as CPU scheduler
- It is responsible for moving processes from *ready queue* to the *CPU*
- It has *lower* the degree of multiprogramming than LST
- It *increases* efficiency

## Medium Term Scheduler

- It moves processes from *waiting queue* to *secondary memory*
- It has the *lowest* degree of multiprogramming
- It is mresponsible for suspending and resuming processes

|                 | Long term scheduler | Short term scheduler | Medium term scheduler |
|-----------------|---------------------|----------------------|-----------------------|
|Queue            |        Job          |        Ready         |       Waiting         |
|Scheduler        |        Job          |         CPU          |  Process Switching    |
|Multiprogramming |      Highest        |        Medium        |       Lowest          |
