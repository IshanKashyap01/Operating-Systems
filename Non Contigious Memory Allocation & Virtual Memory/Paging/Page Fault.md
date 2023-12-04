# Virtual Memory and Page Fault

- Suppose, we have *more pages* than *page frames* available in the RAM

- In order to optimise the allocation of memory pages, the OS reserves some memory
in the *secondary memory* known as **Swap**

- This space is used to store *additional pages* that cannot be stored in the *RAM*
due to lack of storage space

- Whenever a page stored in secondary memory is needed, it will be *swapped* with
an *existing* page in the *RAM*

- The page table will have an *additional bit* to check if the page is *present*
in the RAM

- If the value is set to 0, it means the page is *not present* in the RAM and needs
to be *swapped* to the main memory

- This event is known as **Page Fault**
