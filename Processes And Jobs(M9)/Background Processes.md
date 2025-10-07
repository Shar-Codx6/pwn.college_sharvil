# Background Processes
This level's run wants to see another copy of itself running, not suspended, and using the same terminal. How? Use the terminal to launch it, then suspend it, then background it with bg and launch another copy while the first is running in the background!
## My solve
**Flag:** `pwn.college{EAKXdK85rMRWZdVLGH3JVNcRWs8.QX3QDO0wyM2EzNzEzW}`

```bash
hacker@processes~backgrounding-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!

UID          PID STAT CMD
root         168 S+   bash /challenge/run
root         170 R+   ps -o user=UID,pid,stat,cmd

I don't see a second me!

To pass this level, you need to suspend me, resume the suspended process in the
background, and then launch a new version of me! You can background me with
Ctrl-Z (and resume me in the background with 'bg') or, if you're not ready to
do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~backgrounding-processes:~$ bg
[1]+ /challenge/run &
hacker@processes~backgrounding-processes:~$

Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out.

hacker@processes~backgrounding-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!

UID          PID STAT CMD
root         168 S    bash /challenge/run
root         178 S    sleep 6h
root         179 S+   bash /challenge/run
root         181 R+   ps -o user=UID,pid,stat,cmd

Yay, I found another version of me running in the background! Here is the flag:
pwn.college{EAKXdK85rMRWZdVLGH3JVNcRWs8.QX3QDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
I ran the process /challenge/run. Then I suspended it and ran it in the background by typing bg. After running the process again, I got the flag.
## References 
None