# Practing Piping

## Redirecting More Output
This challenge focuses on redirecting the standard output (stdout) of an executable program to a specific file. The program `/challenge/run` will only grant the flag if its stdout is redirected to a file named `myflag`.

### Solve
**Flag:** `pwn.college{ofH42AVFKXqeRfoeU6ZZfKW9YBu.QX1YTN0wCO5EzNzEzW}`
I obtained the flag by running the /challenge/run program and using the standard output redirection operator `>` to send its output to the specified file, myflag. Then I used cat to display it.

```bash
/challenge/run > myflag
cat myflag
```

### New Learnings
I learnt how to use `>` operator with commands

### References 

