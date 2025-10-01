# Terminal Multiplexing

## Launching Screen
This challenge introduces screen, a terminal multiplexer that creates virtual terminal sessions within a single terminal window, similar to tabs in a web browser. The goal for this level is simply to launch a screen session, as the flag is configured to be immediately displayed upon entering the session.

### Solve
**Flag:** `pwn.college{IeDFtw_lTLiUTuntLT9bHk2c4_Y.0VN4IDOxwCO5EzNzEzW}`

I solved this by executing the screen command. The system was configured to display the flag immediately upon starting the new virtual terminal session.

```bash
screen
```

### New Learnings
I learned the basic function and execution of the screen command.

### References
