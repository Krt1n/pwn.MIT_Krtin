# The File System

## Implicit Relative Path

### Solve
**Flag:** `pwn.college{A6S3hrB6gXfZDOXTXc7U4Wbw8PC.QX4QTN0wCO5EzNzEzW}`

Here the relative path was present in the root file, so we just directly access / first and then access challenge/run (No Need of cd as they are in the same file)

```bash
~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/zoneinfo/posix/Asia directory.
Please use the `cd` utility to change directory appropriately.
~$ cd /usr/share/zoneinfo/posix/Asia
$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{A6S3hrB6gXfZDOXTXc7U4Wbw8PC.QX4QTN0wCO5EzNzEzW}
```

### New Learnings
Root is /, Basically is the places where are the files are present. 
The cd command changes your current location, which affects how you use relative paths to navigate.
Relative Paths just access the file directly in a particular directory (No use of cd)
### References 

