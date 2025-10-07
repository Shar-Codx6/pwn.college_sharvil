# Listing Processes
In this level, I have once again renamed /challenge/run to a random filename, and this time made it so that you cannot ls the /challenge directory! But I also launched it, so you can find it in the running process list, figure out the filename, and relaunch it directly for the flag!
## My solve
**Flag:** `pwn.college{EG5cEF96Ki1qsNM8_tFPteGQNeP.QX4MDO0wyM2EzNzEzW}`

```bash
hacker@processes~listing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.0   1056   640 ?        Ss   13:31   0:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace
root           7  0.0  0.0 231708  2560 ?        S    13:31   0:00 /run/dojo/bin/sleep 6h
root         132  0.0  0.0   4132  2560 ?        S    13:31   0:00 /challenge/31172-run-24148
root         135  0.0  0.0   2744  1600 ?        S    13:31   0:00 sleep 6h
hacker       146  0.0  0.0  36972 21760 ?        Sl   13:31   0:00 /nix/store/g0q8n7xfjp7znj41hcgrq893a9m0i474-ttyd-1.7.7/bi
hacker       150  0.0  0.0 231940  4160 pts/0    Ss+  13:31   0:00 /run/dojo/bin/bash --login
hacker       160  0.1  0.0 231576  3520 pts/1    Ss   13:32   0:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interact
hacker       166  0.0  0.0 231940  4160 pts/1    S    13:32   0:00 /run/dojo/bin/bash --login
hacker       175  0.0  0.0 233600  3840 pts/1    R+   13:32   0:00 ps aux
hacker@processes~listing-processes:~$ /challenge/31172-run-24148
Yahaha, you found me! Here is your flag:
pwn.college{EG5cEF96Ki1qsNM8_tFPteGQNeP.QX4MDO0wyM2EzNzEzW} 
Now I will sleep for a while (so that you could find me with 'ps')
```
## Incorrect tangents I went on
None
## What I learned
I first used ps aux to check which processes are running. Then I figured out the file name /challenge/31172-run-24148 and ran it to get the flag.
## References 
None