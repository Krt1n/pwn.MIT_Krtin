# Practing Piping

## Grepping Stored Results
The goal is to redirect the vast output of the /challenge/run program into a file named /tmp/data.txt. This file will contain hundreds of thousands of lines, one of which is the flag. You must then use grep to quickly search the file and extract the flag.


### Solve
**Flag:** `pwn.college{Icnv2ofFN7ovttQcZrR1wPv0Xjt.QX4EDO0wCO5EzNzEzW}`
I executed the `/challenge/run` program and used the `>` operator to redirect its entire output (stdout) into the file `/tmp/data.txt`.
I then used the `grep` command to search the contents of `/tmp/data.txt` for the string `pwn`

```bash
/challenge/run > /tmp/data.txt
grep pwn /tmp/data.txt
```

### New Learnings


### References 

