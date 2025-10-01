# Chaining Commands

## Understanding Shebangs
For this challenge, create a script at /home/hacker/solve.sh that has a proper shebang and output "hack the planet". Remember to make it executable, then run /challenge/run to verify your script works correctly!

### Solve
**Flag:** `pwn.college{oB4BCNW9CVYAsqMBNhuYpEUyxu6.0VOxMDOxwiNzAzNzEzW}`

In this challenge, I used `echo '#!/bin/bash' > solve.sh` to keep the it a shebang file. Next, I ran `echo 'echo "hack the planet"' >> solve.sh` to append it to the file and then I used `chmod` and changed the permission for it to be executable and ran `/challenge/run` and got the flag.

```bash
echo '#!/bin/bash' > solve.sh
echo 'echo "hack the planet"' >> solve.sh
chmod u=rwx solve.sh
/challenge/run
```

### New Learnings
Learned about shebangs.
