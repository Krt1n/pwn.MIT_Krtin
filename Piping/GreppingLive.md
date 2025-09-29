# Practing Piping

## Grepping Live Output
The goal is to pipe the output of /challenge/run (which contains thousands of lines, including the flag) directly into the grep command to search for and extract the flag. Pipe operator (|).


### Solve
**Flag:** `pwn.college{0c_Y-tUfQ1FW3xZn_yeAs2TcEIX.QX5EDO0wCO5EzNzEzW}`
I solved this by using the pipe operator (|) to connect the output of /challenge/run directly to the input of grep.
```bash
/challenge/run | grep pwn.college
```

### New Learnings
The pipe operator is essential for command chaining.

### References 

