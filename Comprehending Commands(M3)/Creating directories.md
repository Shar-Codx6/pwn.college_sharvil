# Creating Directories
The challenge asks us to create a directory `/tmp/pwn` and create a file in it named `college`. Then execute **/challenge/run** to get the flag.
## My solve
**Flag:** `pwn.college{IbuW0RH7FZs-WZt32WXxouF7r5A.QXxMDO0wyM2EzNzEzW}`

```bash
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ ls
college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{IbuW0RH7FZs-WZt32WXxouF7r5A.QXxMDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
Learned how to create a directory and adding files in it.
## References 
None