# Shell Variables

## Printing Exported Variables
The env command prints a list of all variables that have been marked for inheritance by child processes. The flag is stored in the exported environment variable named FLAG, and the goal is to execute env and find the flag in its output.

### Solve
**Flag:** `pwn.college{8oBwD-21OZbobTdKGHhx_azvNhz.QX4UTN0wCO5EzNzEzW}`

```bash
env
pwn.college{8oBwD-21OZbobTdKGHhx_azvNhz.QX4UTN0wCO5EzNzEzW}
```

### New Learnings
The env command is a useful tool for viewing all exported environment variables (which are available to child processes).
It is a faster alternative to using echo $FLAG if you don't know the exact variable name.

### References 

