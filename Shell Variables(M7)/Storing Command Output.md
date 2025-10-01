# Challenge Name
 Read the output of the /challenge/run command directly into a variable called PWN, and it will contain the flag!
## My solve
**Flag:** `pwn.college{IhqIfhiXoC2zc9slcfjOcfhFqwO.QX1cDN1wyM2EzNzEzW}`

```bash
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{IhqIfhiXoC2zc9slcfjOcfhFqwO.QX1cDN1wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
I learned how to store the output of a command in variable.
## References 
None