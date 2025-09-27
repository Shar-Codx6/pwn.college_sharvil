# Help for Builtins
The challenge asks us to use to argument  **help** which shows how a builtin command works. Using this knowledge, find the flag.
## My solve
**Flag:** `pwn.college{MJYlrZvI8o_fqmGAxUOHuexYop8.QX0ETO0wyM2EzNzEzW}`

```bash
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "MJYlrZvI".
hacker@man~help-for-builtins:~$ challenge --secret MJYlrZvI
Correct! Here is your flag!
pwn.college{MJYlrZvI8o_fqmGAxUOHuexYop8.QX0ETO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
Learned how to use **help** argument.
## References 
None
