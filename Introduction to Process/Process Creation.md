# How OS creates a Process

1. OS loads the program and its *static data* to the main memory (RAM)
    - Static data is the data required to initialise the program

2. OS will allocate *run time stack*
    - This run time stack is used by the program for local variables, function
    parameters and returns

3. OS will allocate the *heap memory*
    - This heap memory will be used by program to store dynamic variables
    - OS will grant additional heap memory if the program runs out of it and
    requests more

4. OS will complete tasks related to I/O
    - In Unix, OS will open three file descriptors
    - These are Input, Output and Error descriptors

5. OS will go to the main function of the program and pass the control of CPU to
the program
    - Once the program starts running on the CPU, it becomes a process
