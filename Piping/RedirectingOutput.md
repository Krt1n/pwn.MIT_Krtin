# Practing Piping

## Redirecting Output
This challenge introduces standard output (stdout) redirection to a file using the > character. The goal is to use output redirection to write the string "PWN" (all uppercase) into a file named "COLLEGE" (all uppercase).

### Solve
**Flag:** `pwn.college{czSBc7INY2YDUvQ5sZo1u4NEYnT.QX0YTN0wCO5EzNzEzW}`

I solved this by using the echo command to generate the string "PWN" and redirecting that string's standard output into a file named COLLEGE using the > operator.

```bash
echo PWN > COLLEGE
pwn.college{czSBc7INY2YDUvQ5sZo1u4NEYnT.QX0YTN0wCO5EzNzEzW}
```

### New Learnings
I learned how to use the > operator for output redirection in the shell. 

### References 

