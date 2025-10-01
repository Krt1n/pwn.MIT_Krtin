# Terminal Multiplexing

## Switching Windows (tmux)
We've created a tmux session with two windows:

Window 0 has the flag!
Window 1 has your warm welcome.
Go get that flag!

### Solve
**Flag:** `pwn.college{olT5nEgI_QvUc_pE8cY6jd4eTK_.0FM5IDOxwiNzAzNzEzW}`

In this challenge, I used `tmux a` command to attach to tmux which gave a welcome message and used `ctrl+b 0` to switch to window 0 and got the flag.

```bash
tmux a
ctrl+b 0
```

### New Learnings
Learned how to switch windows using tmux.
