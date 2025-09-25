# Documentation

## Learning Complex Usage
The challenge involves a program called `/challenge/challenge` which is used to print the contents of a file. The program requires the `--printfile` argument, which itself takes another argument: the path to the file you want to read. To solve the challenge, you need to use this command with the correct path to the flag file.

### Solve
**Flag:** `pwn.college{Ib1P2SGyuAVsRPL9hxiDjW0FY4x.QX1ITO0wCO5EzNzEzW}`
By running /challenge/challenge with the --printfile not-the-flag argument, I instructed it to read the file for me, successfully revealing the flag.

```bash
cat not-the-flag
/challenge/challenge --printfile not-the-flag
```

### New Learnings
I learned that you can sometimes access a program to access files you don't have direct permission to read using complex arguements
### References 

