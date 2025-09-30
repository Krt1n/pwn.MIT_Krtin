# Data Manipulation

## Translating Characters
The goal is to pipe the program's output into tr and use it to swap the casing back to its original state, revealing the correct flag.


### Solve
**Flag:** `pwn.college{4KNhWMimm7K-DLjbUzfEigFMiIr.01MxEzNxwCO5EzNzEzW}`

I solved this by piping the output of `/challenge/run` directly into the `tr` command, using character ranges to define the case-swapping translation.

```bash
/challenge/run | tr 'a-zA-Z' 'A-Za-z'
```

### New Learnings
The tr command  is used (translate or delete characters) to modify a stream of data.
Specifically, the combined range `'a-zA-Z'` and the reversed replacement range `'A-Za-z'`

### References 

