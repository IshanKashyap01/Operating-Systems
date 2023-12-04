# Advantages & Disadvantages of Segmentation

## Pros

1. There is no *internal fragmentation* as no extra space is assigned

2. It saves memory as the *code segment* will have **only one copy** in the main
memory by making it **read only** so it is completely isolated
    - This is done by using **protection bits** that defines the permissions for
    a segment

3. It uses memory much more *efficiently*, hence *increasing degree of multiprogramming*

## Cons

1. It suffers from *external fragmentation* as there may be free memory b/w segments
that is too small to be utilised by any process

2. It will have *overhead* due to extra base and bound registers and protection bits
