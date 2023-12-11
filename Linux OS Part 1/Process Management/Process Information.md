# Listing Process Information

## Process Status (ps)

    $ ps -ef | grep sleep
    ishan        405     348  0 20:08 pts/0    00:00:00 sleep 3000
    ishan        411     348  0 20:08 pts/0    00:00:00 grep --color=auto sleep

- **ps** reports a snapshot of the current processes
- **-ef** tag displays information in a full format
- **-el**  lists various states associated with each process on your system
- **less** to view output in page format
- **head** to view the first ten lines
- **grep** is used to search for a matching pattern

## Process Details

    $ echo $$
    348
    $ echo $PPID
    347
    $ pidof sleep
    405
    $ pgrep -l init
    2 init-systemd(Ub
    5 init
    $ pgrep -la init
    2 /init
    5 plan9 --control-socket 6 --log-level 4 --server-fd 7 --pipe-fd 9 --log-truncate

- **echo** **$$** returns the *PID* of the *shell*
- **echo $PPID** returns the *PPID* of the *shell*
- **pgrep -l** (process) gives all *PIDs* for the process
- **pgrep -la** (process) provides more details
- **top** command to view details of resource utilisation
- **glances** provides a more detailed view of resource utilisation
