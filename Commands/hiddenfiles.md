# Commands

## moving files
Interestingly, ls doesn't list all the files by default. Linux has a convention where files that start with a . don't show up by default in ls and in a few other contexts. To view them with ls, you need to invoke ls with the -a flag. We have to find the flag, hidden as a dot-prepended file in /.

### Solve
**Flag:** `pwn.college{0xru6bZy_XvTdFlInCJcB--kdHR.QXwUDO0wCO5EzNzEzW}`
Firstly I changed my directory, then I searched for flag from the list given. Found a suitable match and checked it's contents using cat.

```bash
hacker@commands~hidden-files:~$ ls -a
.  ..  .bash_history  .cache  .config  .local  delete_me  f
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv           bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-2717711602827  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-2717711602827
pwn.college{0xru6bZy_XvTdFlInCJcB--kdHR.QXwUDO0wCO5EzNzEzW}
```

### New Learnings
ls -a is used to find hidden files.
### References 

