# Priority Specification

    $ nice
    0
    $ sleep 300 & ps -el | grep sleep
    [1] 448
    0 S  1000     448     355  0  80   0 -   802 hrtime pts/0    00:00:00 sleep
    $ nice sleep 300 & ps -el | grep sleep
    [1] 453
    0 S  1000     453     355  0  90  10 -   802 hrtime pts/0    00:00:00 sleep

- **nice** returns the *default* priority
- **nice** (process) sets a higher default priority
- **nice -n (priority) (process)** sets a user defined priority
