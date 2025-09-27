# Helpful Programs
The challenge wants us to use the **--help** to find the arguments to get the flag.
## My solve
**Flag:** `pwn.college{gNrxPj3mQPDHqC8BT9UysAZx8rq.QX3IDO0wyM2EzNzEzW}`

```bash
hacker@man~helpful-programs:~$ --help /challenge/challenge
bash: --help: command not found
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 389
hacker@man~helpful-programs:~$ /challenge/challenge -g 389
Correct usage! Your flag: pwn.college{gNrxPj3mQPDHqC8BT9UysAZx8rq.QX3IDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
Learned the usage of **--help**.
## References 
None