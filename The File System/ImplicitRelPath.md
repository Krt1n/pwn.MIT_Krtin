# The File System

## Implicit Relative Path Without /
In this level, we'll practice referring to paths using . a bit more. This challenge will need you to run it from the /challenge directory. Here, things get slightly tricky.
Linux explicitly avoids automatically looking in the current directory when you provide a "naked" path. 

### Solve
**Flag:** `pwn.college{k8BLX8SDt4tpuTBqvPkz6Fxtj4B.QXwUTN0wCO5EzNzEzW}`

Can't use run command directly, So I use relative path to access the run using ./ where dot is basically the challenge 

```bash
~$ /challenge/run
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ .run
bash: .run: command not found
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{svnKO44kZ5CfUjWTZrNY6ixq0au.QXxUTN0wCO5EzNzEzW}
```

### New Learnings
Root is /, Basically is the places where are the files are present. 
The cd command changes your current location, which affects how you use relative paths to navigate.
Relative Paths just access the file directly in a particular directory (No use of cd)
### References 

