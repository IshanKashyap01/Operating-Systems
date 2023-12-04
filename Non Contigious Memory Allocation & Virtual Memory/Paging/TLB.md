# Translation Lookaside Buffers (TLB)

- It is a *h/w cache* used to store entries from *page table*

- **TLB** is **100** times faster than *RAM* and **1000** times faster than *disk*

- As page table is stored in *RAM*, using TLB makes the process much faster

## Process of Resolving VPN

1. CPU will first check the *TLB*, if it contains the entry, then its a *hit* else
its a *miss*

2. In case of a miss, it will check the *Page table*

3. If the page is in the page table, it will add that entry to the *TLB*
