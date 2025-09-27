# File Globbing 

## Matching with *
This challenge introduces globbing using the * wildcard. The * matches any sequence of characters (except for / or a leading .). The goal is to use globbing to change the current directory to /challenge using an argument of at most four characters, and then execute /challenge/run to get the flag.

### Solve
**Flag:** `pwn.college{U2z3Lzd-GWlH1qa6jk55za6g2pA.QXxIDO0wCO5EzNzEzW}`
The challenge required using globbing to navigate to /challenge with an argument of four characters or less.
The shortest and most effective way to match /challenge is with /ch*
I have mentioned all the possible was to run the final command too!
```bash
cd /ch*
/ch*/run
/ch*/ru*
/ch*/r*
```

### New Learnings
I learned the use of the * wildcard for globbing in the shell.
I learned that * can be used to significantly shorten commands, such as using /ch* to stand for /challenge/
### References 

