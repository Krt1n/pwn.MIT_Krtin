# Practing Piping

## Redirecting Errors
This challenge focuses on standard input (stdin) redirection using the < character. The program /challenge/run requires you to redirect a file named PWN into its standard input. This file must contain the string "COLLEGE" (all uppercase).


### Solve
**Flag:** `pwn.college{MXIMt4jY_8LaOOM4aeyGom_zgB-.QXwcTN0wCO5EzNzEzW}`
I used the echo command to write string, `COLLEGE`, into a new file `PWN`.
I then executed the `/challenge/run` program and used the input redirection operator (<) to feed the contents of the PWN file into the program's standard input.

```bash
echo COLLEGE > PWN
/challenge/run < PWN
```

### New Learnings
Learned how to use the `<` operator for input redirection, a crucial concept for feeding the contents of a file directly into a program's
standard input.

### References 

