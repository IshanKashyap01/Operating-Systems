# Linux Namespace

- On Linux, *resource isolation* is implemented using *namespaces* i.e, no process
will affect anything outside its namespace

- It can be used to create **microservices** by isolating every service

- We can create namespaces in terms of the following:
  - file system
  - PID
  - IPC
  - Hostname or domain name
  - UID or GID
  - Network interfaces
  - Cgroup

- As the first process after start-up is **/sbin/init**, it will start in the
*root namespace*

- Suppose, we decide to create a new namespace wrt PID, from a certain process

- The first process to start in a *new* namespace will get the *PID of 1* for
that namespace

- Hence, there can be processes with same PID outside the namespace but they do
not know of each other

```bash
unshare --fork --pid --mount-proc -u /bin/sh
```

- **unshare** runs program in new namespaces
- **--fork** creates a new process
- **--pid** creates *PID tree isolation*
