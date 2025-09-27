# File Globbing 

## Matching with []
The goal is to first navigate to /challenge/files and then execute /challenge/run, providing a single argument that is three characters or less and uses two * globs to match every file that contains the letter 'p'.


### Solve
**Flag:** `pwn.college{UyUWBz_5jrs90WMHEkIQObCguPm.QXzIDO0wCO5EzNzEzW}`
The first * matches any characters before the 'p'. 
This 'p' ensures the letter is present.
The second * matches any characters after the 'p'.


```bash
cd /challenge/files
/challenge/run *p*
```

### New Learnings
The pattern `*<char>*` is a standard, efficient method for searching for a substring.
### References 

