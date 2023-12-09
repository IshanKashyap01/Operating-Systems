# Introduction to Paging

- The physical memory is divided into *equal and fixed size units* known as
**page frames**

- The *virtual memory* is also divided into *fixed size units* known as **pages**

- Each *page frame* will contain a *single virtual memory page*

- In other words, the size of *a page frame and a page* is the **same**

- The OS will use a **page table** to map *pages* and *page frames* to each other

## Problems with Paging

1. It takes more space because of the *page table*

2. The overhead of converting virtual to physical requires a lot of *memory references*
that takes a lot of time making it slow
