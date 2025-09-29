# Practing Piping

## Filtering with grep -v
This challenge focuses on using the grep -v option (invert match) to filter out unwanted output. The goal is to pipe the program's output into grep -v to exclude all lines containing "DECOY" thereby isolating the true flag.

### Solve
**Flag:** `pwn.college{AwI-NCso5rUKd64sBGpsxp57hYN.0FOxEzNxwCO5EzNzEzW}`
I solved this by using the pipe operator to send the massive output stream from `/challenge/run` directly into the `grep` command, using the -v option to invert the match. This allowed me to filter out the noise and isolate the correct flag.

```bash
/challenge/run | grep -v DECOY
pwn.college{AwI-NCso5rUKd64sBGpsxp57hYN.0FOxEzNxwCO5EzNzEzW}
```

### New Learnings
I learned the practical use of grep -v (invert match). 

### References 

