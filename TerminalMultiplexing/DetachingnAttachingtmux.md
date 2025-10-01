# Terminal Multiplexing

## Detaching and Attaching (tmux)
For this challenge:
We Launch tmux, then Detach from it.
Run `/challenge/run` (this will send the flag to your detached session!)
Reattach to see your prize.

### Solve
**Flag:** `pwn.college{EG05cHZoMp70wiNcyRGl6VNj0fk.0VO4IDOxwiNzAzNzEzW}`

In this challenge, I used `tmux` command to launch tmux and detached from it using `ctrl+b d` and then attached back using `tmux` and got the flag.

```bash
tmux
ctrl+b d
tmux a-
```

### New Learnings
Learned how to detach and attach using tmux.
