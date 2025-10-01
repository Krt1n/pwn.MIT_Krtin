# Chaining Commands

## Redirecting Script Output
In this level, we will practice piping (|) from your script to another program. Like before, you need to create a script that calls the `/challenge/pwn` command followed by the /challenge/college command, and pipe the output of the script into a single invocation of the `/challenge/solve` command!

### Solve
**Flag:** `pwn.college{gB1cuYQODRS4O6Pseg1dwxVUnuv.QX4ETO0wiNzAzNzEzW}`

In this challenge, I ran used `echo` with argument `/challenge/pwn; /challenge/college` onto `x.sh` and used bash on it with pipe operator `| /challenge/solve` and got the flag.

```bash
echo "/challenge/pwn; /challenge/college" > x.sh
bash x.sh | /challenge/solve
```

### New Learnings
Learned about shell script output.
