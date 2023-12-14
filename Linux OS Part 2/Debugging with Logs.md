# Debugging using Logs

    journalctl may be used to query the contents of the systemd(1) journal as
    written by systemd- journald.service(8).

    If called without parameters, it will show the full contents of the journal,
    starting with the oldest entry collected.

    If one or more match arguments are passed, the output is filtered accordingly

- **-u** followed by a service name to search the logs
- **-f** Show only the most recent journal entries, and continuously print new entries
as they are appended to the journal

        dmesg - print or control the kernel ring buffer
        DESCRIPTION
            dmesg is used to examine or control the kernel ring buffer.

            The default action is to display all messages from the kernel ring buffer

- It shows all the device driver messages and can be used to debug h/w devices
