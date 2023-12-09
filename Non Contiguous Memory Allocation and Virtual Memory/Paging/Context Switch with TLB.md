# Context Switch with TLB

- A process can have multiple pages, and each of them usually starts from 0 to n

- So, any two processes can have the different pages with the *same VPN*

- Now suppose there are two processes in the RAM P1 and P2, with **10** pages each

- Let's say, P1 is running and both of them have page number *10* stored in the
*TLB*

- Now, P1 needs I/O operations to be done so the OS context switches to P2 and
requests for *page 10* of P2

- However, there are *two* entries in the *TLB* with the *VPN of 10* and no way
of knowing which one corresponds to the current process\

## Solution 1: Flush the TLB

- Every time a context switch occurs, empty the TLB so there are no duplicate values

- However, OS rapidly switch processes every second

- Therefore, the TLB will be flushed every switch and filled at the start of a
process only to be flushed again rendering it a useless overhead

## Solution 2: Add a Process Identifier (ASID)

- Add an **Address Space Identifier (ASID)** to each entry to identify the *process*
to which the *page* belongs to

- This *ASID* can uniquely identify *all* entries in the *TLB*

- This way, there is *no need* to flush the TLB, it can be always full and used
to maximum affect

- Moreover, *ASID* is of **8 bits**, making it more efficient to use than *PID*,
which is of **32 bits**
