# Address Translation

- The *address translation* is calculated by using the formula:

    **physical address = base + offset**

- The *offset* represents the required address in the *virtual memory*  

- It is calculated by using the formula:

    **offset = starting address - required address**

- As *stack* grows in *upwards direction*, its offset value will always be **negative**

- Hence, the *bound register* will *subtract* its value from *base* to get the *range*

- If the process requests an address *b/w heap and stack*, it will be given a
**segmentation error** also known as **segmentation fault**

## Identification of Segment

- For a given address, OS must be able to know which segment of the process it belongs

- A *virtual address* is represented in the form of **14 bits**

- The OS assigns the *first two bits* as a *unique identifier*
