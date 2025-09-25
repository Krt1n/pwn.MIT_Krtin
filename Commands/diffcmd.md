# Commands

## comparing files
Sometimes, the files that you might cat out are too big. Luckily, we have the grep command to search for the contents we need! We'll learn it in this challenge.Invoked like this, grep will search the file for lines of text containing SEARCH_STRING and print them to the console.

### Solve
**Flag:** `pwn.college{kcdE9CYNVy9jKww1G-3nRVic7SN.01MwMDOxwCO5EzNzEzW}`
WE have to change the directory to challenge and then just use the diff command to compare b/w both the files.

The file is located in the flag directory, so we just use the command to 
```bash
~$ cd /challenge
:/challenge$ diff decoys_only.txt decoys_and_real.txt
56a57
> pwn.college{kcdE9CYNVy9jKww1G-3nRVic7SN.01MwMDOxwCO5EzNzEzW}
```

### New Learnings
diff compares two files line by line and shows what's different between them.
56a57 means after line 56 of file add line 57 
### References 

