# Practing Piping

## Duplicating piped data with tee
This challenge focuses on using an alternative argument to the tee command to achieve the desired pipe and file output. The goal is to pipe the output of `/challenge/pwn` into `/challenge/college`, but first, you must use tee to intercept and save the output of `/challenge/pwn` to a file. This file will contain the secret argument required to make `/challenge/pwn` generate the actual flag data for `/challenge/college`.

### Solve
**Flag:** `pwn.college{oar7vsoLMX9FDrlkXZ5_OAjcxhh.QXxITO0wCO5EzNzEzW}`
Used tee to debug the interaction and then executing the final correct command chain. I used tee temp in the initial pipe to save the output of `/challenge/pwn`, which revealed the required secret was `oar7vsoL`

```bash
/challenge/pwn | tee temp | /challenge/college
cat temp
/challenge/pwn --secret [SECRET_ARG]
SECRET_ARG should be "oar7vsoL"
/challenge/pwn --secret oar7vsoL | /challenge/college
pwn.college{oar7vsoLMX9FDrlkXZ5_OAjcxhh.QXxITO0wCO5EzNzEzW}
```

### New Learnings
Learnt the use of the tee command. It acts as a "T-splitter" in a pipe, duplicating the data stream: sending one copy to the next command in the pipe and another to one or more files. 

### References 

