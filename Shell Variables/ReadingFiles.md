# Shell Variables

## Reading Files
This challenge focuses on efficiently reading the contents of a file directly into a shell variable using the read builtin and input redirection (<).The goal is to read the content of the file /challenge/read_me into the variable named PWN.

### Solve
**Flag:** `pwn.college{kz5ulVd165sKXM6xjIo7x88Cmsl.QXwIDO0wCO5EzNzEzW}`

I solved this by combining the read builtin with input redirection (<).

```bash
export PWN
read PWN < /challenge/read_me
pwn.college{kz5ulVd165sKXM6xjIo7x88Cmsl.QXwIDO0wCO5EzNzEzW}
```

### New Learnings
Learnt a more efficient method for reading file contents into a variable using: `read VAR < FILE`

### References 
["The Useless Use of the Cat"](https://porkmail.org/era/unix/award#cat)
