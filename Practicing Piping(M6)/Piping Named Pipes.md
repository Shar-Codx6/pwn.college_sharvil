# Piping Named Pipes
This challenge will be a simple introduction to FIFOs. You'll need to create a /tmp/flag_fifo file and redirect the stdout of /challenge/run to it. If you're successful, /challenge/run will write the flag into the FIFO! Go do it!
## My solve
**Flag:** `pwn.college{YNzDSjJGTA4Uf1vexyf1xS4nnCX.01MzMDOxwyM2EzNzEzW}`
Console 1:
```bash
hacker@piping~named-pipes:~$ mkfifo /tmp/flag_fifo
hacker@piping~named-pipes:~$ /challenge/run > /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo!
Bash will now try to open the FIFO for writing, to pass it as the stdout of
/challenge/run. Recall that operations on FIFOs will *block* until both the
read side and the write side is open, so /challenge/run will not actually be
launched until you start reading from the FIFO!
```
Console 2:
```bash
hacker@piping~named-pipes:~$ cat /flag_fifo
cat: /flag_fifo: No such file or directory
hacker@piping~named-pipes:~$ cat /tmp/flag_fifo 
You've correctly redirected /challenge/run's stdout to a FIFO at 
/tmp/flag_fifo! Here is your flag:
pwn.college{YNzDSjJGTA4Uf1vexyf1xS4nnCX.01MzMDOxwyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
I learned how to create a pipe and what are its conditions to accept the operations on FIFO.
## References 
None