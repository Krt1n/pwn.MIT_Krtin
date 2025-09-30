# Data Manipulation

## Extracting specific sections of text
This challenge focuses on using the cut command to extract specific columns (fields) of data from a piped stream, then using tr to clean the result. 
The /challenge/run program outputs lines of data separated by spaces, where the flag characters are in a specific column. The goal is to use cut to extract the correct field, then pipe that output to tr -d "\n" to remove newlines and reconstruct the single-line flag.

### Solve
**Flag:** `pwn.college{k3IbXcQCRzNhQOdBznk6uBOo_Ra.01NxEzNxwCO5EzNzEzW}`

I solved this by chaining three commands using pipes: `/challenge/run` to generate the data, `cut` to isolate the flag characters, and `tr -d "\n"` to remove the newlines and form the final flag string.

```bash
/challenge/run | cut -d " " -f 2 | tr -d "\n"
```

### New Learnings
Syntax: `cut -d "DELIMITER" -f FIELD_NUMBER`
I learned the core functionality of the cut command for column extraction, which requires specifying a delimiter (-d) and the field number (-f) to extract.

### References 

