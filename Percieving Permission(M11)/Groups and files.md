# Groups and files
In this level, I have made the flag readable by whatever group owns it, but this group is currently root. Luckily, I have also made it possible for you to invoke chgrp as the hacker user! 
## My solve
**Flag:** `pwn.college{441-0d8t3mh0zrIXFR8CNP3mkcA.QXxcjM1wyM2EzNzEzW}`

```bash
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{441-0d8t3mh0zrIXFR8CNP3mkcA.QXxcjM1wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
explain what you learned

## References 
None