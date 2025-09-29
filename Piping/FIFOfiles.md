# Practing Piping

## Named Pipes
The goal is to create a FIFO named /tmp/flag_fifo and then redirect the standard output of /challenge/run into this FIFO. To complete the write operation, you must simultaneously read from the FIFO in a separate step or terminal, which will unblock the write operation and reveal the flag.

### Solve
**Flag:** `pwn.college{8LYTSVmk4jkFE-jV2ugk0R6sQ22.01MzMDOxwCO5EzNzEzW}`
I solved this by creating a FIFO and then executing the redirect and the read operations in the same terminal session, using the blocking behavior of the FIFO.

```bash
mkfifo /tmp/flag_fifo
/challenge/run > /tmp/flag_fifo  # Run in background in one terminal
cat /tmp/flag_fifo               # And run in foreground in a second terminal
```

### New Learnings
This challenge introduces Named Pipes (or FIFOs, First In, First Out), which are file-like objects that allow inter-process communication directly in memory, without using disk storage.
FIFOs block (wait) until both a process is reading from it and a process is writing to it. 
`mkfifo` command: makes a fifo file. [indicated by a p in ls -l].
### References 

