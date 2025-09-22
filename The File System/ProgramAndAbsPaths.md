# The File System

## Program and Absolute Paths
 The name of the challenge program in this level is run, and it lives in the /challenge directory. Thus, the path to the run challenge program is /challenge/run.

### Solve
**Flag:** `pwn.college{cA6yXaOBpmix41NuGYth77v_mf9.QX1QTN0wCO5EzNzEzW}`

The / indicates root file, here we access the subfolder challenge and then access run

```bash
~$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{cA6yXaOBpmix41NuGYth77v_mf9.QX1QTN0wCO5EzNzEzW}
```

### New Learnings
Root is /, Basically is the places where are the files are present. 
Here we learn to access the subfolders.
To run an executable file, all we have to do is paste the path.
### References 

