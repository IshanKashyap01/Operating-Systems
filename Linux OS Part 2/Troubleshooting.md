# Troubleshooting in Linux

    du -chs *

    NAME
       du - estimate file space usage

    DESCRIPTION
       Summarize disk usage of the set of FILEs, recursively for directories.

       Mandatory arguments to long options are mandatory for short options too.

        -c, --total
            produce a grand total
        -h, --human-readable
            print sizes in human readable format (e.g., 1K 234M 2G)
        -s, --summarize
            display only a total for each argument

- Using an asterisk at the end of the command will report usage of each directory/file

- **rm -rf** to remove files from a directory; using an "*" will delete all the files

- **find** command is used to search files in a directory with syntax:

        find location -type d -name directory
        find location -type n -name file

- **diff** command is used to compare two files line by line
