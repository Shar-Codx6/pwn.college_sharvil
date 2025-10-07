# Other users with su
In this level, you must switch to the zardus user and then run /challenge/run. Zardus' password is dont-hack-me.
## My solve
**Flag:** `pwn.college{ITQx3xra0tLFVln_42PNIEQYevq.QX2UDN1wyM2EzNzEzW}`

```bash
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# cat /flag
pwn.college{YRrmUAD-_5s4an5Ex9gByb1zfDQ.QX1UDN1wyM2EzNzEzW}
root@users~becoming-root-with-su:/home/hacker#
Connected!
hacker@users~other-users-with-su:~$ su zardus
Password:
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{ITQx3xra0tLFVln_42PNIEQYevq.QX2UDN1wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned

## References 
None