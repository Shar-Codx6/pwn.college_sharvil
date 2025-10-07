# Suspeding Processes
This level's run wants to see another copy of itself running and using the same terminal. How? Use the terminal to launch it, then suspend it, then launch another copy while the first is suspended
## My solve
**Flag:** `pwn.college{4oYgT9iG0uuD0s7O4aqIiDcNbdI.QX1QDO0wyM2EzNzEzW}`

```bash
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         161     129  0 14:21 pts/0    00:00:00 bash /challenge/run
root         163     161  0 14:21 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         161     129  0 14:21 pts/0    00:00:00 bash /challenge/run
root         168     129  0 14:21 pts/0    00:00:00 bash /challenge/run
root         170     168  0 14:21 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{4oYgT9iG0uuD0s7O4aqIiDcNbdI.QX1QDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
Suspending Process is basically creating a copy of a process which will keep running in the foreground.
## References 
None