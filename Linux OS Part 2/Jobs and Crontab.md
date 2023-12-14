# Jobs and Crontab

## Jobs Command

    jobs: jobs [-lnprs] [jobspec ...] or jobs -x command [args]
        Display status of jobs.

        Options:
        -l        lists process IDs in addition to the normal information
        -n        lists only processes that have changed status since the last
                    notification
        -p        lists process IDs only
        -r        restrict output to running jobs
        -s        restrict output to stopped jobs


    $ sleep 3600 & sleep 4600 & sleep 5600 & ping google.com
    [1] 626
    [2] 627
    [3] 628
    PING google.com (142.250.193.142) 56(84) bytes of data.
    64 bytes from maa05s25-in-f14.1e100.net (142.250.193.142): icmp_seq=1 ttl=113
    time=53.3 ms
    ^Z
    [4]+  Stopped                 ping google.com

    $ jobs -l %p
    [4]+   629 Stopped                 ping google.com

## Crontab Command

- It is used to schedule jobs to run regularly
- It provides option of time, date, month and day of the week

## Archiving with tar Command

    tar cfz xy.tar.gz xy

- **c** to create an archive, **f** to specify tar we're creating an archive and
**z** to *zip* this directory

- **xy.tar.gz** is name of the archive, and **xy** is the directory
