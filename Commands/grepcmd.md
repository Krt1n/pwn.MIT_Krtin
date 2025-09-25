# Commands

## grepping for a needle in a haystack
Sometimes, the files that you might cat out are too big. Luckily, we have the grep command to search for the contents we need! We'll learn it in this challenge.Invoked like this, grep will search the file for lines of text containing SEARCH_STRING and print them to the console.

### Solve
**Flag:** `pwn.college{8YZUynrCyFnlaLb_OKs_EE2Ln5L.QX3EDO0wCO5EzNzEzW}`

The file is located in the flag directory, so we just use the command to 
```bash
~$ grep pwn.college /challenge/data.txt
pwn.college{8YZUynrCyFnlaLb_OKs_EE2Ln5L.QX3EDO0wCO5EzNzEzW}
```

### New Learnings
Grep searches the file for lines of text containing SEARCH_STRING and print them to the console.
### References 

