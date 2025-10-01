# Chaining Commands

## Handling Failure
In this challenge, you need to chain `/challenge/first-failure` and `/challenge/second` using the `||` operator. Go for it!

### Solve
**Flag:** `pwn.college{og7S3W6hhvJI_3Hf7nLGeU0WHct.01M0MDOxwiNzAzNzEzW}`

In this challenge, I ran `/challenge/first-failure` separated by `||` and `/challenge/second` to get the flag.

```bash
/challenge/first-failure || /challenge/second
```

### New Learnings
Learned about handling failure `||`.
