# Data Manipulation

## Deleting New Lines
The `/challenge/run` program outputs the flag, but with newlines injected throughout, splitting the flag across multiple lines. 
The goal is to pipe the output into tr -d and use the escaped character `\n` to delete the newlines, turning the output into a single, complete flag string.

### Solve
**Flag:** `pwn.college{4LIot1iDZeRHBCeGWOUMpITBOwS.0VNxEzNxwCO5EzNzEzW}`

Solved this by piping the output directly into the tr command, using the -d option.
The escaped newline was enclosed in quotes ("\n") to prevent the shell from interpreting the newline and to ensure it was passed correctly to tr as the character to delete.

```bash
/challenge/run | tr -d %^
```

### New Learnings
I learned how to use escaped characters in the shell, specifically \n for the newline character

### References 

