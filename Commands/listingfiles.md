# Commands

## listing files
ls will list files in all the directories provided to it as arguments, and in the current directory if no arguments are provided.

### Solve
**Flag:** `pwn.college{wooCvsPNWWrj9h6zS0tBaoqgUGJ.QX4IDO0wCO5EzNzEzW}`
WE have to change the directory to challenge and then we found the renamed file and by accessing the renamed file gives access to the flag

```bash
hacker@commands~listing-files:/challenge$ ls
20128-renamed-run-3417  DESCRIPTION.md
hacker@commands~listing-files:/challenge$ /challenge/20128-renamed-run-3417
Yahaha, you found me! Here is your flag:
pwn.college{wooCvsPNWWrj9h6zS0tBaoqgUGJ.QX4IDO0wCO5EzNzEzW}
```

### New Learnings
Ls command listing the directories or files for a particular directory.
### References 

