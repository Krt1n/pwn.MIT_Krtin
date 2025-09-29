# Practing Piping

## Writing To Multiple Programs
The goal is to run /challenge/hack and duplicate its output stream into the standard input of both /challenge/the and /challenge/planet commands. This requires the output to be duplicated and delivered at the same time.This challenge extends Process Substitution to allow writing to multiple commands simultaneously using the tee command and the output process substitution syntax (>(command))

### Solve
**Flag:** `pwn.college{UI4TgZg0RiQb-Kz_ydVCnafwHFy.QXwgDN1wCO5EzNzEzW}`
I solved this by chaining the /challenge/hack command with tee, using output process substitution for the two target commands.

```bash
/challenge/hack | tee >(/challenge/the) >(/challenge/planet)
```

### New Learnings
Learnt the function of output process substitution, which uses the syntax >(command). This feature runs a command and provides a special file path (a named pipe) that, when written to, sends the data to the command's standard input.

### References 

