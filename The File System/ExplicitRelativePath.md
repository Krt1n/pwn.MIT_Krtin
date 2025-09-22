# The File System

## Explicit Relative Path
Previously, your relative path was "naked": it directly specified the directory to descend into from the current directory. In this level, we're going to explore more explicit relative paths. We will be using . and ..

### Solve
**Flag:** `pwn.college{k8BLX8SDt4tpuTBqvPkz6Fxtj4B.QXwUTN0wCO5EzNzEzW}`

We first access the root file as they have given that it is the current working directory, then I access the run using relative path where . just indicates the root directory here

```bash
~$ /challenge/run
hacker@paths~explicit-relative-paths-from-:/challenge$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./run
bash: ./run: Is a directory
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{k8BLX8SDt4tpuTBqvPkz6Fxtj4B.QXwUTN0wCO5EzNzEzW}
```

### New Learnings
Root is /, Basically is the places where are the files are present. 
The cd command changes your current location, which affects how you use relative paths to navigate.
Relative Paths just access the file directly in a particular directory (No use of cd)
### References 

