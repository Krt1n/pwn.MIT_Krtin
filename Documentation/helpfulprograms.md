# Documentation

## Helpful Programs
Some programs lack a man page, but instead provide a built-in help menu, often accessible with the --help or -h arguments.

### Solve
**Flag:** `pwn.college{EeYiXL2g5iqOzSO2s8fe3wj83tz.QX3IDO0wCO5EzNzEzW}`
My first step was to run /challenge/challenge --help, which provided a detailed usage guide.
The guide listed a -p that reveals the correct value for the -g. 
I used -p to find the secret value (252) and then used -g 252 to get the flag.

```bash
/challenge/challenge --help
/challenge/challenge -p
/challenge/challenge -g 252
```

### New Learnings
This challenge highlighted the importance of using a program's built-in help menu (--help or -h) when no man page is available.
### References 

