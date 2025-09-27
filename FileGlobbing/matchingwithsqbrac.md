# File Globbing 

## Matching with []
The goal is to navigate to the /challenge/files directory and then execute /challenge/run with a single argument that uses the bracket glob to match the four files: file_b, file_a, file_s, and file_h. The program requires the use of the bracket glob in the argument.


### Solve
**Flag:** `pwn.college{UyUWBz_5jrs90WMHEkIQObCguPm.QXzIDO0wCO5EzNzEzW}`
 I changed the directory to the location of the target files: cd /challenge/files.
 The files all start with file_ and end with one of the characters: a, b, s, or h. I constructed the glob pattern file_[absh] to match any single character from that set.

```bash
cd /challenge/files
/challenge/run file_[absh]
```

### New Learnings
Unlike the ? wildcard which matches any single character, [] is a powerful tool for specifying a limited set of acceptable characters for a single position in a filename. Allows for targeted matching of multiple files simultaneously.
### References 

