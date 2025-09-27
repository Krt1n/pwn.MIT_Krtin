# File Globbing 

## Tab Completion on Commands
This challenge focuses on using tab completion for commands rather than files. The goal is to find and execute a command that starts with pwncollege by typing the prefix and using the Tab key to automatically complete the rest of the command name.

### Solve
**Flag:** `pwn.college{U5gNGX9hzBnudL2rnOXuTF8Ggf0.0VN0EzNxwCO5EzNzEzW}`
I started typing pwncollege and pressed Tab, which expanded the command to pwncollege-4668 (or a similar randomly generated number).

```bash
pwncollege<TAB>
pwncollege-4668
```

### New Learnings
I learned that tab completion is not limited to file paths; it is also a powerful tool for completing executable command names. 
### References 

