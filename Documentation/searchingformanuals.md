# Documentation

## Serching For Manuals
The challenge is to find a hidden man page with a randomized name. This man page contains the instructions needed to run a specific program, /challenge/challenge, to get the flag. To find the hidden man page, you must learn how to search the man page database using the man command itself. The hint is to read man man, which will teach you.

### Solve
**Flag:** `pwn.college{wBYX_ZtQH_O7BCQxUIHIS7n6W5O.QX2EDO0wCO5EzNzEzW}`
The challenge required using the man -K command to search for the hidden man page. It is given that /challenge/challenge is the search term. The correct man page was the one that provided the unique argument wtxnwz and the specific number 776

```bash
man -K /challenge/challenge
/challenge/challenge --wtxnwz 776
```

### New Learnings
This challenge demonstrated the power of the man -K (or --apropos) command. It allows for a global keyword search across all installed man pages, which is essential for finding documentation when the exact name of the manual is unknown.
### References 

