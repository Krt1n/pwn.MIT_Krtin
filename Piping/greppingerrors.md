# Practing Piping

## Grepping Errors
This challenge focuses on redirecting standard error (stderr) so it can be processed by a pipe (|). Since the pipe operator only processes standard output (stdout, FD 1), the goal is to use the 2>&1 operator to redirect stderr (FD 2) into stdout. The combined output stream is then piped into grep to find the flag, which is being outputted over stderr.


### Solve
**Flag:** `pwn.college{ArcSqFuhKHETeu-7QFMVvbBwhif.QX1ATO0wCO5EzNzEzW}`
The key to solving this was using the 2>&1 operator to merge the standard error (FD 2) into the standard output (FD 1).

```bash
/challenge/run 2>&1 | grep pwn.college
```

### New Learnings
I learned the powerful technique of redirecting one file descriptor to another using the `FD2>&FD1` syntax. It can also be the other way around.

### References 

