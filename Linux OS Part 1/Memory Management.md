# Memory Management

## CGroups

    $ ls /sys/fs/cgroup/
    blkio  cpu,cpuacct  cpuset   freezer  memory  net_cls           net_prio    pids
    systemd
    cpu    cpuacct      devices  hugetlb  misc    net_cls,net_prio  perf_event  rdma
    unified

- It is a mechanism used to limit the maximum resources available to a process
or a group of processes

- **/sys/fs/cgroup** contains all the different files to manage the system
- **memory** directory can be used to manage memory

- If we create a folder in the *memory* directory, the system will automatically
add some files necessary for memory management

- These files are used to manage the memory of a process
