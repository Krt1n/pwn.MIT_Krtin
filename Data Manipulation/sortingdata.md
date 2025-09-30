# Data Manipulation

## Sorting Data
This challenge focuses on using the sort command to organize data and isolate the real flag. A file at `/challenge/flags.txt` contains 100 fake flags mixed with the single, genuine flag. The challenge states that when the file is sorted alphabetically, the real flag will be the last line. The goal is to sort the file to reveal the flag.

### Solve
**Flag:** `pwn.collegd{IWaGVQcCJ795Dk1p-JX6RVytvjc.0EM0LDOxwCO5EzNzEzW}`

I used reverse sort (-r), the first line of the output is the last line of the alphabetical sort.Which in turn gives us the the flag as the first one when in reverse.

```bash
sort /challenge/flags.txt
# OR
sort /challenge/flags.txt | tail -n 1
```

### New Learnings
I learned the basic functionality of the sort command, which performs an alphabetical sort by default. I also learned the -r option for reverse order sorting.

### References 

