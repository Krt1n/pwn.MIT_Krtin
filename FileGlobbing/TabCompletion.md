# File Globbing 

## Tab Completion
This challenge focuses on the utility and safety of tab completion as an alternative to globbing. The flag is located in the file /challenge/pwncollege, but the filename has been created with a hidden, non-printable character, making it impossible to type out manually. You must use tab completion to correctly enter the filename and read the flag with cat.


### Solve
**Flag:** `pwn.college{A8uY9INrQcjN--B8BHWPxl96-jE.0FN0EzNxwCO5EzNzEzW}`
The key to solving this was to use tab completion to overcome the hidden character in the filename. The initial attempts to cat /challenge/pwncollege failed because the file listed by ls (pwncollege) contained an invisible, non-printable character.

```bash
hacker@globbing~tab-completion:~$ cat /challenge/pwncollege​
pwn.college{A8uY9INrQcjN--B8BHWPxl96-jE.0FN0EzNxwCO5EzNzEzW}
```

### New Learnings
Tab completion is not only a faster way to type commands and file paths but is also essential for correctly accessing files that contain non-printable or tricky characters.
### References 

