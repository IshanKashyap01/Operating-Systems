# Virtual Address Representation & Translation

## Virtual Address Representation

- Suppose we have a main memory of 128 KB divided into eight page frames but
we only have *four pages*

- So, each *page* will be of *16 KB* and total size will be *64 KB*

- Any address of any *page* can be represented using **6 bits** as *2^6 = 64*

- Similarly, any address in a page can be represented by **4 bits**

- Say, we want the *21st KB* in the *virtual memory*, so its address will be
**01 0101**

- The *first two bits* represents the *page* and the remaining *four bits* represent
its *location within the page*

- The bits representing the *page* are known as **Virtual Page Number (VPN)**

- The remaining bits are known as **offset**

- The *VPN* for each *page* is a *unique ID* assigned by the OS

- In this case, the IDs will be **00, 01, 10 and 11**, hence, the address belongs
to the *first page*

## Address Translation

- The OS will identify the *page frame* of the *virtual address*

- This will be done via the *page table* using the *VPN* of the address

- The *VPN* will be converted to the **Page Frame Number (PFN)** and the *offset*
will remain the same

- Suppose, the *first page* is mapped to the *seventh frame*

- Therefore, the *VPN* i.e, **01** (1) will be converted to **111** (7)

- Hence, the physical address will be **111 0101** (117)

- Meaning, the *21st KB* in the *virtual address* is the *117th KB* in the *physical*
*memory*
