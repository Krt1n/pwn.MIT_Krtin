# File Globbing 

## Matching with ?
The goal is to use ? in the argument to cd to match the /challenge directory, replacing characters like 'c' and 'l', and then execute /challenge/run to get the flag.


### Solve
**Flag:** `pwn.college{0pSGCFhhxOmh236-esExIr0wLZy.QXyIDO0wCO5EzNzEzW}`
I solved this by using the ? wildcard to replace specific characters in the /challenge path. The command cd /?ha??enge successfully expanded to /challenge. After navigating to the correct directory, executing /challenge/run revealed the flag.

```bash
cd /?ha??enge
/challenge/run
```

### New Learnings
I learned the difference between the * and ? globbing wildcards: ? is strictly a single-character wildcard, making it useful for matching file or directory names with only a single unknown character.
### References 

