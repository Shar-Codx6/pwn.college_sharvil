# Interrupting processes
In this challenge, /challenge/run will refuse to give you the flag until you interrupt it.
## My solve
**Flag:** `pwn.college{Quxw_K0IDEQhvV243G8w94b5eCE.QXzQDO0wyM2EzNzEzW}`

```bash
hacker@processes~interrupting-processes:~$ /challenge/run
I could give you the flag... but I won't, until this process exits. Remember,
you can force me to exit with Ctrl-C. Try it now!
^C
Good job! You have used Ctrl-C to interrupt this process! Here is your flag:
pwn.college{Quxw_K0IDEQhvV243G8w94b5eCE.QXzQDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
I understood how to use the command ctrl+C to exit a process instead of killing it everytime.
## References 
None