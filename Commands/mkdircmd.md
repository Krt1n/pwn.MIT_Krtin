# Commands

## An Epic File System Quest
This challenge tests your ability to navigate and interact with a Linux filesystem using a series of clues. Each clue provides a path to the next location and a hint on how to find the next clue, requiring you to use different commands and options to progress.

### Solve
**Flag:** `pwn.college{Aw-ZWb_hvYbAw3LN-48E8vNHLmE.QXxMDO0wCO5EzNzEzW}`
I used the mkdir command to create the directory, followed by cd to enter it. I then used touch to create the empty college file. Finally, I ran the /challenge/run script, which found the file and provided the flag.

```bash
mkdir /tmp/pwn
cd /tmp/pwn
touch college
/challenge/run
```

### New Learnings
I learned how to use the `mkdir` command to create a directory
### References 

