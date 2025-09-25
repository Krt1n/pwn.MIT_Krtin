# Commands

## An Epic File System Quest
This challenge tests your ability to navigate and interact with a Linux filesystem using a series of clues. Each clue provides a path to the next location and a hint on how to find the next clue, requiring you to use different commands and options to progress.

### Solve
**Flag:** `pwn.college{wvnAQgV45nUAkDheeQMk3WQWWu7.QX5IDO0wCO5EzNzEzW}`

I solved this by following the chain of clues provided. Each clue gave me a path to the next location and a method to find the next file, such as using ls -a for hidden files, using cd for delayed files, and using an absolute path with cat for trapped files.

```bash
cd /
cat NOTE
cd /opt/linux/linux-5.4/drivers/staging
ls -a
cat .SPOILER
cd /usr/lib/python3/dist-packages/jedi/third_party/typeshed/third_party/2and3/pymysql/constants
ls -a
cat LEAD
cd /usr/local/lib/python3.8/dist-packages/sympy/tensor/array/expressions/tests/__pycache__
ls -a
cat DISPATCH
cd /opt/linux/linux-5.4/Documentation/networking/device_drivers/qualcomm
ls -a
cat ALERT
ls /usr/share/perl/5.30.0/Test2/IPC/Driver
cat /usr/share/perl/5.30.0/Test2/IPC/Driver/TEASER-TRAPPED
cd /usr/local/lib/python3.8/dist-packages/prompt_toolkit/contrib/completers
ls
cat TIP
cd /usr/lib/aspell/x86_64-linux-gnu
ls -a
cat .CLUE
cd /usr/share/javascript/mathjax/jax/output/SVG/fonts/Gyre-Termes/Normal
ls
cat README
```


### New Learnings
I learned to identify different types of filesystem puzzles and how to use commands like ls -a and cat with absolute paths to solve them.
### References 

