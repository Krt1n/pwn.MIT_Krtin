# Chaining Commands

## Scripting with Arguments
For this challenge, you need to write a script at `/home/hacker/solve.sh` that:
    -Takes two arguments
    -Outputs them in REVERSE order (second argument first, then the first argument)

### Solve
**Flag:** `pwn.college{YsEr_Dj8Y_hhnpJ7UUUo-dYLC61.0VNzMDOxwiNzAzNzEzW}`

In this challenge, I appended `echo "$2 $1"` into the `solve.sh` file so that if it takes 2 arguments it prints argument 2 first then argument 1 and I ran `/challenge/run` to get the flag.

```bash
nano solve.sh
echo "$2 $1"
/challenge/run
```

### New Learnings
Learned about scripting with arguments.
