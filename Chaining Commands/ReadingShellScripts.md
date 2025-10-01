# Chaining Commands

## Reading Shell Scripts
In this level, we will learn to read shell scripts. `/challenge/run` is a shell script that requires you to put in a secret password, but that password is hardcoded into the script iself! Read the script figure out the password, and get the flag!

### Solve
**Flag:** `pwn.college{kVQq0sgRrkE0FI0UH175Lh-YpNc.0lMwgDOxwzNzAzNzEzW}`

In this challenge, I ran `echo "hack the PLANET"` onto the file using pipe operator `|` and got the flag.

```bash
echo "hack the PLANET" | /challenge/run
```

### New Learnings
Learned about reading shell scripts.
