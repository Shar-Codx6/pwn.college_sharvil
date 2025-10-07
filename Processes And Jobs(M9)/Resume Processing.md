# Resume Processing
This challenge requires to first suspend the run process and then resume it using fg.
## My solve
**Flag:** `pwn.college{0WZAZ56I1dLSE0iJcaLX4H_sx-A.QX2QDO0wyM2EzNzEzW}`

```bash
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[2]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg
/challenge/run
I'm back! Here's your flag:
pwn.college{0WZAZ56I1dLSE0iJcaLX4H_sx-A.QX2QDO0wyM2EzNzEzW}
Don't forget to press Enter to quit me!

Goodbye!
```
## Incorrect tangents I went on
None
## What I learned
I learned how to resume a process again after suspending.
## References 
None