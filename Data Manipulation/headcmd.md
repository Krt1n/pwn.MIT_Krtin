# Data Manipulation

## Extracting the first lines with head
This challenge focuses on using the head command to limit the piped output from one command before sending it to another.
We must pipe this output through head to grab exactly the first 7 lines and then pipe those 7 lines to the `/challenge/college` program, which will validate the input and provide the flag.

### Solve
**Flag:** `pwn.college{M0TgVjpeNVGw8hLAzMiO8gd7t05.0lNxEzNxwCO5EzNzEzW}`

The head -n 7 command was placed in the middle of the pipe to act as a filter, taking the full output from /challenge/pwn and passing only the first 7 lines to the standard input of /challenge/college.

```bash
/challenge/pwn | head -n 7 | /challenge/college
```

### New Learnings
I learned how to use the head command with the -n option to control the exact number of lines read from a data stream.

### References 

