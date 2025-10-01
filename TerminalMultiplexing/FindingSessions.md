# Terminal Multiplexing

## Launching Screen
This challenge focuses on listing and reattaching to specific screen sessions. As an avid user may have multiple sessions, the screen -ls command is used to list all active sessions. The goal is to identify the correct session out of three decoy sessions, reattach to it using `screen -r` `<session_name_or_PID>`, and find the one that contains the flag. 

### Solve
**Flag:** `pwn.college{UxtEuBo6ohVh29bBGSr-vOPYMgG.01N4IDOxwCO5EzNzEzW}`

I solved this by using the screen -ls command to list all three active sessions. I then iteratively used screen -r with each session's PID or name to attach, checked the content for the flag, and detached (Ctrl-A d) to return to the parent shell.

```bash
screen -ls
screen -r <SessionID_1>
# Press Ctrl-A, then d
screen -r <SessionID_2>
# Press Ctrl-A, then d (repeat until flag is found)
echo pwn.college{UxtEuBo6ohVh29bBGSr-vOPYMgG.01N4IDOxwCO5EzNzEzW}
```

### New Learnings
I learned how to manage multiple screen sessions using screen -ls to list all sessions (showing the PID and session name) and `screen -r <ID>` to reattach to a specific session.

### References
