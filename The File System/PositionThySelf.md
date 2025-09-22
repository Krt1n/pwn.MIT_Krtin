# The File System

## Position Thy Self
 The name of the challenge program in this level is run, and it lives in the /challenge directory. Thus, the path to the run challenge program is /challenge/run.

### Solve
**Flag:** `pwn.college{023jvbEDU0QbaaKot_Sq2bLybU9.QX2QTN0wCO5EzNzEzW}`

First I ran the original path, since it returned invalid and also returned the path where it exsists, I used cd to access it and run the command.

```bash
~$ /challenge/run
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/doc directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /usr/share/doc
hacker@paths~position-thy-self:/usr/share/doc$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{023jvbEDU0QbaaKot_Sq2bLybU9.QX2QTN0wCO5EzNzEzW}
```

### New Learnings
Root is /, Basically is the places where are the files are present. 
The cd command changes your current location, which affects how you use relative paths to navigate.
Learnt to figure out a path when original path of file is not given.
To run an executable file, all we have to do is paste the path.
### References 

