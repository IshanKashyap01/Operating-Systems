# Storage Allocation Methods

## Contiguous Allocation

- All blocks of a file are stored continuously as the number of blocks required
by the file are *estimated* beforehand

- *Performance* is *very fast* as we only have to move to the next block

- Estimation of size may be wrong leading to *fragmentation*

## Linked Allocation

- All the blocks of a file are connected as a *linked list*

- Directory containing the file will have the *head and tail* of the list

- However, each block will have to store additional *pointer(s)* for the list

- Moreover, we can access blocks in a *sequential manner only*

- Loss of pointer in case of singly LL will lead to file corruption

## Indexed Allocation

- An *extra block* is used to store *pointers* to *all the blocks* of the file

- This block is known as the **index block**

- *Direct access* to any block is possible and loss of one pointer will not lead
to file corruption

- However, it uses more pointers and the overhead caused is greater

- If the file is small, the index block will have a lot of wasted space
