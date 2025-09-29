# Shell Variables

## Exporting Variables
This challenge introduces the concept of exporting variables so they are passed to child processes (like /challenge/run). Variables are local by default. The goal is to: Set the variable PWN to COLLEGE and export it & Set the variable COLLEGE to PWN but do not export it (keep it local).

### Solve
**Flag:** `pwn.college{UzvUXa1SMdcYq92_hxFtuCmTjh3.QXyYTN0wCO5EzNzEzW}`
I used export PWN=COLLEGE to set the variable and pass it to the child process's environment.
I used COLLEGE=PWN to set the variable locally without exporting it.

```bash
export PWN=COLLEGE
COLLEGE=PWN
/challenge/run
```

### New Learnings
The export command is essential for promoting a local variable into the shell's environment, ensuring that its value is inherited by any child processes (like programs or scripts) that the current shell runs. 
Variables set without export remain local to the current shell.

### References 

