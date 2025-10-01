# Chaining Commands

## Scripting with Default Cases
For this challenge, write a script at `/home/hacker/solve.sh` that:
    Takes one argument
    -If the argument is "pwn", output "college"
    -For any other input, output "nope"

### Solve
**Flag:** `pwn.college{80Q2yzN_2QWANuLJo1Ab4dlGR96.01NzMDOxwiNzAzNzEzW}`

In this challenge, I first appended the entire `if then else fi` condition into `solve.sh` then tried running with pwn as argument and no argument which worked. So, I ran `/challenge/run` and got the flag.

```bash
bash solve.sh pwn
bash solve.sh
/challenge/run
```

### New Learnings
Learned about scripting with default cases.
