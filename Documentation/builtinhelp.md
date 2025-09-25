# Documentation

## Help For Builtin
Some commands are shell builtins and are handled directly by the shell instead of being external programs. This challenge requires you to use the help command to find the correct argument for the challenge builtin to get the flag.

### Solve
**Flag:** `pwn.college{QKHWVeZu0HwcD3smtgSQQcC3Ii5.QX0ETO0wCO5EzNzEzW}`
My first step was to run help challenge, which provided a detailed usage guide for the challenge builtin. The help text explained that the --secret option required a specific value, QKHWVeZu, to print the flag. 

```bash
help challenge
challenge --secret QKHWVeZu
```

### New Learnings
Shell builtins and learned to use the help command to get documentation for these builtins
### References 

