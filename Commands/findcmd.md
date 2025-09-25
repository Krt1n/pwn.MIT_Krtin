# Commands

## finding files


### Solve
**Flag:** `pwn.college{Y0S8GTgoKmnHVM_RahSd7HGgyni.QXyMDO0wCO5EzNzEzW}`
I began by using the find command to locate all files named flag on the system. I randomly chose one of the paths to inspect. My initial attempt to cd into /usr/share/locale/sl/flag failed, as indicated by the "Not a directory" error. Realizing it was a file, I used cat with the full path to read its contents, which revealed the flag.

```bash
find / -name flag
cat /usr/share/locale/sl/flag
```

### New Learnings
I learnt how to use the find command in linux.
### References 

