# Practing Piping

## Spliting Standard Error and Standard Output
This challenge requires mastering an advanced redirection technique: splitting the standard output (stdout) and standard error (stderr) streams from a single program and routing each stream into the standard input of a separate program. 
You must run `/challenge/hack` and redirect its stdout to `/challenge/planet` and its stderr to `/challenge/the`.

### Solve
**Flag:** `pwn.college{klN9ivk-smqg-KqPkPltx4g9rQ8.QXxQDM2wCO5EzNzEzW}`
The expressions >(/challenge/planet) and >(/challenge/the) are executed first by the shell. 
`1>` Redirects stdout of  to the named pipe.
`2>` Redirects stderr of to the named pipe.

```bash
/challenge/hack 1> >(/challenge/planet) 2> >(/challenge/the)
```

### New Learnings
Learnt the combination of FD Redirection (1>, 2>) with Output Process Substitution (>(command))
### References 

