# Removing Files
The challenge asks us to create a **delete_me** file and delete it using `rm`. Then execute `/challenge/check` to get the flag.

## My solve
**Flag:** `pwn.college{0JpTQ0cq4iZEIYI3ttWs60J6phI.QX2kDM1wyM2EzNzEzW}`

```bash
hacker@commands~removing-files:~$ touch delete_me
hacker@commands~removing-files:~$ ls
 delete_me   key   key.pub  '~'
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{0JpTQ0cq4iZEIYI3ttWs60J6phI.QX2kDM1wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
Learned how to delete files in your home directory.
## References 
None