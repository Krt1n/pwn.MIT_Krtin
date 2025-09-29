# Practing Piping

## Redirecting More Output
This challenge focuses on appending standard output (stdout) to a file using the `>>` operator, as opposed to overwriting it with `>`. The program /challenge/run writes the flag in two parts: the first part directly to the target file, and the second part to stdout. 

The goal is to run /challenge/run and redirect its output to /home/hacker/the-flag using append mode (>>) so that the second part of the flag is added after the first part.

### Solve
**Flag:** `pwn.college{oXxcihBioYgwWjDla9pbNSR27wn.QX3ATO0wCO5EzNzEzW}`
I solved this by using the append redirection operator `>>`.This ensured that the second write from the program's stdout was appended to the file.

```bash
/challenge/run >> /home/hacker/the-flag
cat the-flag
```

### New Learnings
The `>>` operator is essential for adding new output to an existing file without deleting its current contents.

### References 

