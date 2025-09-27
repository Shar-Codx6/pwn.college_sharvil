# Reading Manuals
The challenge first asks us to use the **man** command to see the details of **/challenge** program. Using the details, use the argument to find the flag.
## My solve
**Flag:** `pwn.college{grYHIXTkLmP6F_mTEug3bTyMWn8.QX0EDO0wyM2EzNzEzW}`

```bash
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ man /usr/bin/challenge
It looks like you're trying to run 'man' with an absolute path to the command.
That isn't how man works! Instead, man references a centralized database of
manpages, and fetches one based on a name, not a file path. So to pull up the
man page for the program '/bin/ls', you would run 'man ls', not 'man /bin/ls'.
hacker@man~reading-manuals:~$ man ls
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge --grkmmu
Incorrect usage! Please read the challenge man page!
hacker@man~reading-manuals:~$ /challenge/challenge --grkmmu 638
Correct usage! Your flag: pwn.college{grYHIXTkLmP6F_mTEug3bTyMWn8.QX0EDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
I learned how to use the man command.
## References 
None