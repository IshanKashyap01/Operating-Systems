# Running a Process

    $ sleep 300 &
    [1] 415
    $ jobs
    [1]+  Running                 sleep 300 &
    $ fg %1
    sleep 300
    ^Z
    [1]+  Stopped                 sleep 300
    $ bg
    [1]+ sleep 300 &

- The *&* operator is used to run the process in *background*
- **jobs** lists the processes running in background and gives each a *job id*
- **fg %**(job id) brings it to *foreground*
- **bg** sends it to *background*
