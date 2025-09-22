# The File System

## Home Sweet Home
Every user has a home directory, typically under /home in the filesystem. In the dojo, you are the hacker user, and your home directory is /home/hacker. The home directory is typically where users store most of their personal files. As you make your way through pwn.college, this is where you'll store most of your solutions.
The ~ in this prompt is the current working directory, with ~ being shorthand for /home/hacker. Bash provides and uses this shorthand because, again, most of your time will be spent in your home directory. Thus, whenever bash sees ~ provided as the start of an argument in a way consistent with a path, it will expand it to your home directory.

### Solve
**Flag:** `pwn.college{gWytFrvENJzRdeo5ONs1lUC7tng.QXzMDO0wCO5EzNzEzW}`

It is stated that the program is located at /challenge/run. To get the key we use touch to create a file to store the key. Then we access that file using the ~ operation to go to the home/hacker path
challenge/run: Is where the program is executing. It is located at the absolute path /challenge/run and /home/hacker/f: Is the argument I am providing to the program. It is the path to the file where the program should write its output.

```bash
hacker@paths~home-sweet-home:~$ touch ~/f
hacker@paths~home-sweet-home:~$ /challenge/run ~/f
Writing the file to /home/hacker/f!
... and reading it back to you:
pwn.college{gWytFrvENJzRdeo5ONs1lUC7tng.QXzMDO0wCO5EzNzEzW}
```

### New Learnings
Touch command is used to create a file. 


### References 
Add any references or videos you used while solving the challenge.
