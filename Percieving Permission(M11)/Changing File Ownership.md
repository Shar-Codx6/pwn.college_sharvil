# Chaning file ownership
In this level, we will practice changing the owner of the /flag file to the hacker user, and then read the flag. For this challenge only, I made it so that you can use chown to your heart's content as the hacker user
## My solve
**Flag:** `pwn.college{AqcFIUDyRS_EJ7-dxE65LoTR4dy.QXxEjN0wyM2EzNzEzW}`

```bash
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{AqcFIUDyRS_EJ7-dxE65LoTR4dy.QXxEjN0wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned

## References 
None