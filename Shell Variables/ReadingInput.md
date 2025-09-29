# Shell Variables

## Reading Input
The goal is to execute the read command, prompt for input, and store the value COLLEGE (which you will type) into the variable PWN. The optional -p argument is used to specify a prompt string.

### Solve
**Flag:** `pwn.college{sME9vt_oLZFuxI4Xrb8PWEnz2ns.QX4cTN0wCO5EzNzEzW}`
Used the read builtin along with the -p argument to display a prompt and wait for user input. Input provided was `COLLEGE` 
```bash
read -p "INPUT: " PWN
# User then types: COLLEGE
pwn.college{sME9vt_oLZFuxI4Xrb8PWEnz2ns.QX4cTN0wCO5EzNzEzW}
```

### New Learnings
Learnt how to use the read builtin to capture user input and store it directly into a specified shell variable.

### References 

