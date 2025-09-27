# File Globbing 

## Exclusionary Globbing
When `!` or `^` is the first character inside square brackets, it inverts the match, causing the glob to match any single character not listed.The goal is to navigate to /challenge/files and run /challenge/run with a single argument that uses exclusionary globbing to match all files that do not start with 'p', 'w', or 'n'.


### Solve
**Flag:** `pwn.college{IJqKK8UNkXyuF286SNiyjzrdCzf.QX2IDO0wCO5EzNzEzW}`
`[!pwn]` matches any single character that is not 'p', 'w', or 'n'. `*` matches the rest of the filename.

```bash
cd /challenge/files
/challenge/run [!pwn]*
```

### New Learnings
I learned about exclusionary globbing using the `[!...]` or `[^...]` pattern. 
### References 

