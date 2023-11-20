# Attributes of a Process

- As there are multiple processes running at once, OS stores metadata about each
process in a **Process table**

- Each entry in this table is called a **Process Control Block** (PCB)

## Process Table

The process table stores the following attributes of each process:

### Process ID

A unique identifier for each process.

### Program Counter

Stores the address of the next instruction to be run. OS will incrementing its
value to the next instruction as it fetches the address of the current
instruction.

### Process State

A process will go through multiples states from its start to end. This attribute
stores the present state of a process.

### Priority

Based on the priority, each process will get CPU time.

### General Purpose Register

Used for storing variables used during program execution

### List of Open File

List of files opened by the process

## List of Open Devices

List of open I/O devices used by the process
