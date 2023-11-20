# Architecture of Process

- The memory allocated to a program has the following components:

  - **Stack**: data related to local variables, function parameters and return values
  - **Heap**: memory used for dynamically allocated data
  - **Data**: the global and static data used for initialising the program
  - **Text**: the compiled code

- Heap and Stack are present at the two ends of the allocated memory.

- As the space occupied by them increases, their boundaries draw closer.

- If the stack meets the heap, the OS throws a **stack over flow error**.

- Alternatively, if the program requests more memory for heap, OS will throw an
**insufficient memory error**.
