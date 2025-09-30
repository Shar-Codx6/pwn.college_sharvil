# Redirecting Inputs
 In this level, we will practice using /challenge/run, which will require you to redirect the PWN file to it and have the PWN file contain the value COLLEGE!
## My solve
**Flag:** `pwn.college{E_cAiYPh_k2VubylbG_npAxYoO9.QXwcTN0wyM2EzNzEzW}`

type in your solve and your thought process behind solving the challenge. Include as much as info as possible. Use triple ticks for bash.
```bash
hacker@piping~redirecting-input:~$ echo PWN > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Your PWN file must have the value 'COLLEGE', but I instead read: PWN
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{E_cAiYPh_k2VubylbG_npAxYoO9.QXwcTN0wyM2EzNzEzW}
```
## Incorrect tangents I went on
Redirecint `echo PWN` instead of `echo CHALLENGE`.
## What I learned
I learned how to feed commands into a file.
## References 
None