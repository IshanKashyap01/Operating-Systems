# Components of File System

The file system is implemented in a layered structure. Following are the layers
from bottom to top

- At the lowest level, the **device** is present, which stores the data

- **I/O control** has the device drivers to interact with the h/w

- The **basic file system** works directly with the I/O control

- The **File organisation module** keeps tracks the *mapping* of logical and physical
addresses of the files

- The **logical file system** keeps track of all the *metadata* of the files

- The top most layer, is the **application programs**
