# Multiple Options for Tab Selection
This challenge has a /challenge/files directory with a bunch of files starting with pwncollege. Tab-complete from /challenge/files/p or so, and make your way to the flag!
## My solve
**Flag:** `pwn.college{UAEM321MPMUFCpkDqKYaAqel0q8.0lN0EzNxwyM2EzNzEzW}`

```bash
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwn
No flag in this file!
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwn
pwn                    pwn-the-planet         pwncollege-flag        pwncollege-flyswatter
pwn-college            pwncollege-family      pwncollege-flamingo    pwncollege-hacking
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwn-college
No flag in this file!
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwn-the-planet
No flag in this file!
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-
pwncollege-family      pwncollege-flag        pwncollege-flamingo    pwncollege-flyswatter  pwncollege-hacking
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-family
No flag in this file!
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-fl
pwncollege-flag        pwncollege-flamingo    pwncollege-flyswatter
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-fla
pwncollege-flag      pwncollege-flamingo
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-flag
pwn.college{UAEM321MPMUFCpkDqKYaAqel0q8.0lN0EzNxwyM2EzNzEzW}
```
## Incorrect tangents I went on
Unable to locate the flag quickly
## What I learned
Learned about how to use the option page by tab compeletion

## References 
None