# Documentation

## Serching Manuals
You can scroll man pages with the arrow keys (and PgUp/PgDn) and search with /. After searching, you can hit n to go to the next result and N to go to the previous result. Instead of /, you can use ? to search backwards!

### Solve
**Flag:** `pwn.college{U0hAzqqXGG6vhy4tPIRRJAYKM7s.QX1EDO0wCO5EzNzEzW}`
The challenge required me to find the correct argument for the /challenge/challenge program by reading its manual page. After typing man challenge, I used the / key to search for keywords,then I found the correct argument, --jhiquxd.

```bash
man challenge
/
/challenge/challenge --jhiquxd
```

### New Learnings
I learned how to search within manual pages using the / key.
### References 

