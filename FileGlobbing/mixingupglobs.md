# File Globbing 

## Mixing up Globs
The goal is to navigate to /challenge/files and run /challenge/run, providing a single argument that is six characters or less and matches only the files "challenging", "educational", and "pwning".


### Solve
**Flag:** `pwn.college{kuvkRZ6z04ejJf_riIzsAvaYf3w.QX1IDO0wCO5EzNzEzW}`
I used the bracket glob [cep] to match the unique starting characters, and the * wildcard to match the rest of the filename. 
[cep] matches 'c', 'e', or 'p' (the first letter of the targets).
* matches the rest of the file name.

```bash
cd /challenge/files
/challenge/run [cep]*
```

### New Learnings
I learned how to mix different globbing types ([] and *) to create specific yet concise patterns.
### References 

