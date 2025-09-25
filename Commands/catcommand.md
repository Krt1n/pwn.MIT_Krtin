# Commands

## cat: not the pet, but the command!
In this challenge, I will copy the flag to the flag file in your home directory (where your shell starts). Go read it with cat!

### Solve
**Flag:** `pwn.college{c67jiYWyoYz7KRwXaX3Nu0wu50n.QXxcTN0wCO5EzNzEzW}`

The file is located in the home directory, so no need to change directories, just use the command directory to access the file

```bash
cat flag
pwn.college{c67jiYWyoYz7KRwXaX3Nu0wu50n.QXxcTN0wCO5EzNzEzW}
```

### New Learnings
cat is used for reading out files, if mulitple files are provided it concats both the files

### References 

