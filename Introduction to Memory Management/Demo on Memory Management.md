# Demo on Memory Management

- Suppose, we have a program that does the following:
  - Initialises an integer variable and prints its location on the memory
  - Increments by one and prints its value four times in a row

- If we run two instances of this program *simultaneously*, the memory location
of the variable in both instances will be the *same*

- Consequently, we'd believe that both the programs are using the *same memory*
and incrementing the *same variable*

- Meaning, the output for both instances will be *different* to what it would've
been had we only ran *one instance*

- *However, the output comes out exactly the same*

- This is because the OS assigns a different block of memory to each process but
*neither knows the actual physical location* of that memory

- Instead of knowing the physical address, the processes have a *virtual address*
starting from zero

- This way each process has a simplified memory allocation and the mapping is
done and handled by the OS

- This is known as **virtualisation of memory**
