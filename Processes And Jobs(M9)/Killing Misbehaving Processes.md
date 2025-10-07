# Killing Misbehaving Processes
type what the challenge asks
In this challenge, there's a decoy process that's hogging a critical resource - a named pipe (FIFO) at /tmp/flag_fifo into which (like in the Practicing Piping FIFO challenge) /challenge/run wants to write your flag. You need to kill this process.

Your general workflow should be:

1. Check what processes are running.
2. Find /challenge/decoy in the list and figure out its process ID.
kill it.
3. Run /challenge/run to get the flag
## My solve
**Flag:** `pwn.college{kUjgeFbfdpkQuW5pchOs1j1qIFY.0FNzMDOxwyM2EzNzEzW}`

```bash
hacker@processes~killing-misbehaving-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.0   1056   640 ?        Ss   14:07   0:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace
root           7  0.0  0.0 231708  2560 ?        S    14:07   0:00 /run/dojo/bin/sleep 6h
root         137  0.0  0.0   4132  1280 ?        S    14:07   0:00 /bin/bash /challenge/.init
root         138  0.0  0.0   4132  1280 ?        S    14:07   0:00 /bin/bash /challenge/.init
root         140  0.0  0.0   2744  1600 ?        S    14:07   0:00 sleep 6h
root         141  0.0  0.0   2744  1600 ?        S    14:07   0:00 sleep 6h
hacker       153  0.0  0.0  36972 21760 ?        Sl   14:07   0:00 /nix/store/g0q8n7xfjp7znj41hcgrq893a9m0i474-ttyd-1.7.7/bi
hacker       156  0.0  0.0 231576  3520 pts/0    Ss   14:07   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interact
hacker       162  0.0  0.0 231972  4160 pts/0    S+   14:07   0:00 /run/dojo/bin/bash --login
hacker       172  0.0  0.0 231972  4160 pts/1    Ss+  14:07   0:00 /run/dojo/bin/bash --login
hacker       204  0.1  0.0 231576  3520 pts/2    Ss   14:15   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interact
hacker       210  0.0  0.0 231972  4160 pts/2    S    14:15   0:00 /run/dojo/bin/bash --login
hacker       221  0.0  0.0 233600  3840 pts/2    R+   14:16   0:00 ps aux
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!
hacker@processes~killing-misbehaving-processes:~$ cat /tmp/flag_fifo
pwn.college{kUjgeFbfdpkQuW5pchOs1j1qIFY.0FNzMDOxwyM2EzNzEzW}
```
## Incorrect tangents I went on
I was not able to figure out the real flag in the starting.
## What I learned
I ran ps aux, I found the file /challenge/decoy. I killed the file, ran /challenge/run and then cat the Fifo pipe to get the flag.
## References 
None