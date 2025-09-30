# Redirecting Output
In this challenge, you must use this output redirection to write the word PWN (all uppercase) to the filename COLLEGE (all uppercase).
## My solve
**Flag:** `pwn.college{gM6WOY7uz0yWRX0I8Q2GAlnuz3o.QX0YTN0wyM2EzNzEzW}`

```bash
hacker@piping~redirecting-output:~$ echo PWN > COLLEGE
Correct! You successfully redirected 'PWN' to the file 'COLLEGE'! Here is your
flag:
pwn.college{gM6WOY7uz0yWRX0I8Q2GAlnuz3o.QX0YTN0wyM2EzNzEzW}
hacker@piping~redirecting-output:~$ cat COLLEGE
PWN
You have created the COLLEGE file and wrote the right value to it, but it
doesn't look like you did it via input redirection.
```
## Incorrect tangents I went on
None
## What I learned
I learned that using '>' you can redirect the output to any file and run from there as well.
## References 
None