# Types of Memory

## Stack Memory

- It is used for storing function parameters, local variables and return values
- In other words, stack memory is used to store function calls
- Data is stored in a *continuous* fashion resulting in *faster* operations and
*optimised* storage
- Memory is allocated and deallocated *dynamically* as function calls are made
and resolved *automatically* by the program
- This stack memory is also known as *temporary allocated memory*

## Heap Memory

- It is used for storing dynamically allocated data structures
- Data is stored in a *random* fasion resulting in *slower* operations and is
*less efficiently* managed leading to *fragmentation*
- Allocation and deallocation is managed by the *programmer*
- If the program exits, the data will still remain in the heap memory
- If the programmer forgets to deallocate the memory, it will cause *memory leaks*
