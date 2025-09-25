# Finding files
In the challenge, the flag will be kept in a random directory in the filesystem. I have to use to **find** command to locate the file and look for the flag.
## My solve
**Flag:** `pwn.college{g9X1ZGCOKS_EVjA8CusaCK2Yyky.QXyMDO0wyM2EzNzEzW}`

```bash
hacker@commands~finding-files:~$ find / -name flag
find: ‘/root’: Permission denied
find: ‘/etc/ssl/private’: Permission denied
find: ‘/tmp/tmp.TpSOPGOVKK’: Permission denied
/usr/local/lib/python3.8/dist-packages/wcwidth/flag
/usr/local/lib/python3.8/dist-packages/pwnlib/flag

^C
hacker@commands~finding-files:~$ cat /usr/local/lib/python3.8/dist-packages/wcwidth/flag
pwn.college{g9X1ZGCOKS_EVjA8CusaCK2Yyky.QXyMDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
got confused on how do I check for the content inside /flag.
## What I learned
I learned about finding a file using the syntax `find / -name flag`.
## References 
None