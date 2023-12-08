# Introduction to Concurrency & Threads

- A **thread** is a *sequential flow of control* within a process/program

- Threads of the same process can share some variables/values with each other

- The concept of running multiple threads simultaneously is known as **concurrency**

- While the process of doing so is known as **multithreading**

## Scheduling Issues with Threads

- Imagine there is a shared variable b/w two or more threads and each thread
make changes to its value

- Now suppose, if a thread is preempted while in the middle of a change, and another
thread made a change before control is returned to the former thread

- Here, the former thread will change this variable to a wrong value leading to
unpredictable behaviour

- Therefore, we need to make sure that a thread is not disturbed while it completes
its change
