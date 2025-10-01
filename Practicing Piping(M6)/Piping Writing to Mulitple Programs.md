# Piping writing to multiple programs.
In this challenge, we have /challenge/hack, /challenge/the, and /challenge/planet. Run the /challenge/hack command, and duplicate its output as input to both the /challenge/the and the /challenge/planet commands!
## My solve
**Flag:** `pwn.college{sy4fBMgb4-FvzPLmSoHkwVK2s9u.QXwgDN1wyM2EzNzEzW}`

```bash
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
20060548247329175
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{sy4fBMgb4-FvzPLmSoHkwVK2s9u.QXwgDN1wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
I learned how to store the output of a command in multiple programs using <(command).
## References 
None