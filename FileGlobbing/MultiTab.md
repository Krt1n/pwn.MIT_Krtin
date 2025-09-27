# File Globbing 

## Tab Completion
This challenge focuses on tab completion when multiple options exist. When you press Tab and the partial input could complete to several different files, Bash will complete up to the point of commonality and then, upon pressing Tab a second time, display all matching options. 
The goal is to use this behavior, starting from /challenge/files/p (or similar), to navigate and find the file containing the flag among many files beginning with pwncollege.


### Solve
**Flag:** `pwn.college{sBCuU4j2FkTkTRguARfXeTYUWwR.0lN0EzNxwCO5EzNzEzW}`
I solved this by iteratively using tab completion to narrow down the file options until I found the one that contained the flag.

```bash
cat /challenge/files/pwn
No flag in this file!
cat /challenge/files/pwn
pwn             pwn-the-planet          pwncollege-flag         pwncollege-flyswatter  
pwn-college       pwncollege-family       pwncollege-flamingo     pwncollege-hacking     
cat /challenge/files/pwn-college
No flag in this file!
cat /challenge/files/pwn-the-planet
No flag in this file!
cat /challenge/files/pwncollege-flag
pwn.college{sBCuU4j2FkTkTRguARfXeTYUWwR.0lN0EzNxwCO5EzNzEzW}
```

### New Learnings
Learned how to manage multi-option tab completion in Bash. Pressing Tab once completes the common prefix; pressing Tab again shows all possible completions.
### References 

