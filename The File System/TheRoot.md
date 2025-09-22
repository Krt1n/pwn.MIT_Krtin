# The File System

## The Root
Alright, so the filesystem starts at /. Under that, there are a whole mess of other directories, configuration files, programs, and, most importantly, flags. In this level, we've added a program right in /, called pwn, that will give you the flag. All you need to do for this level is to invoke this program!

### Solve
**Flag:** `pwn.college{ImBdq5YzO7-Xm1AMdCwbyp45tvT.QX4cTO0wCO5EzNzEzW}`

The / indicates root file, so to access pwn program in the root using absolute path we use:

```bash
~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{ImBdq5YzO7-Xm1AMdCwbyp45tvT.QX4cTO0wCO5EzNzEzW}
```

### New Learnings
Root is /, Basically is the places where are the files are present

### References 

