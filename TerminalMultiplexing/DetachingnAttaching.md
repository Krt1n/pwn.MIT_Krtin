# Terminal Multiplexing

## Launching Screen
This challenge focuses on the detach and reattach functionality of the screen terminal multiplexer. This feature allows a user to keep a session and its running programs active in the background even after closing the terminal.

### Solve
**Flag:** `pwn.college{IiVr2zjcN-funKOxK4gCSniap3h.0lN4IDOxwCO5EzNzEzW}`

I solved this by executing the screen command. The system was configured to display the flag immediately upon starting the new virtual terminal session.

```bash
screen
# User presses Ctrl-A, then d
/challenge/run 
screen -r
```

### New Learnings
I learned the practical use of screen's detach/reattach feature. The keyboard shortcut for detaching is Ctrl-A then d, and the command to reattach is screen -r. 

### References
