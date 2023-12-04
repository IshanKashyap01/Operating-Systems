# Page Replacement Policies

## First in First Out (FIFO)

- Processes are removed in the same order as they enter

- However, *hit rate* is *low* as it does not account for how many times pages
are requested and can evict pages in high demand

## Least Recently Used (LRU)

- It keeps track of how recently a page was requested

- It selects the least recently used page to evict out of the main memory

- Hence, the *hit rate* is *high* as pages in high demand remains in memory for
longer
