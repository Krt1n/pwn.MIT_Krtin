# Chaining Commands

## Scripting with Conditionals
For this challenge, write a script at `/home/hacker/solve.sh` that:
    Takes one argument
    -If the argument is "pwn", output "college"
    -For any other input, output nothing

### Solve
**Flag:** `pwn.college{s9qGZaMAbclkgF7csPkfkGQ6x5z.0lNzMDOxwiNzAzNzEzW}`

In this challenge, I first appended the entire `if then fi` conditions into `solve.sh` then tried running with pwn as argument and no argument which worked. So, I ran `/challenge/run` and got the flag.

```bash
bash solve.sh pwn
bash solve.sh
/challenge/run
```

### New Learnings
Learned about scripting with conditionals.
