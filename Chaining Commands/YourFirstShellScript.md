# Chaining Commands

## Your First Shell Script
Same as last level, Run /challenge/pwn and then /challenge/college, but this time in a shell script called x.sh, then run it with bash!

### Solve
**Flag:** `pwn.college{gmq1LLDXmZQMnZbmWG8gX4d0NTN.QXxcDO0wiNzAzNzEzX}`

In this challenge, I ran used `echo` with argument `/challenge/pwn; /challenge/college` onto `x.sh` and bashed it to get the flag.

```bash
echo "/challenge/pwn; /challenge/college" > x.sh
bash x.sh
```

### New Learnings
Learned about shell script.
