# Practing Piping

## Process Substitution
The goal is to use process substitution with the diff command to compare the output of two programs: `/challenge/print_decoys` and `/challenge/print_decoys_and_flag`. The diff output will reveal the single extra line containing the flag.

### Solve
**Flag:** `pwn.college{woUnUU5WhOT52xs7aX9KZQNJcso.0lNwMDOxwCO5EzNzEzW}`
I used the syntax diff <(command1) <(command2) to feed the output of both programs as arguments to diff.

```bash
diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
```

### New Learnings
The syntax for input process substitution is <(command).It runs the specified command and replaces the expression with the path to a special, temporary file.

### References 

