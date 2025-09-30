# Data Manipulation

## Deleting Characters
This challenge focuses on using the tr command with the -d (delete) option to remove specific characters from an input stream. The program /challenge/run outputs the flag, but with decoy characters (% and ^) interspersed throughout. The goal is to pipe the output into tr -d to remove these two characters and reveal the correct flag.


### Solve
**Flag:** `pwn.college{gF2bKQn8n1q0zF9gWGG9e8CQvfU.0FNxEzNxwCO5EzNzEzW}`

Solved this by piping the output of `/challenge/run` into the tr command, using the -d option to delete the unwanted decoy characters.

```bash
/challenge/run | tr -d %^
```

### New Learnings
I learned the function of the tr -d option, which is used to delete specific characters from standard input.

### References 

