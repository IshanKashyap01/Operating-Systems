# Shortest Job First (SJF)

- This algorithm picks the process with the least BT to run
- The kernel keeps a history of processes and how long they ran
- Using this information it predicts the BT before hand
- However, if a lower BT process comes after a higher BT process is already sent
to the CPU, it will trigger a *convoy effect*
