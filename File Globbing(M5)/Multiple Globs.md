# Multiple globs
The challenge requires to use two * globs and run /challenge/run with single argument that covers every word that contains letter p.
## My solve
**Flag:** `pwn.college{MtjTmD917H-tfR7vLWfpkua1vNB.0lM3kjNxwyM2EzNzEzW}`

```bash
hacker@globbing~multiple-globs:~$ cd /challenge/files
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run /**
Your expansion did not expand to the requested files (happy optimistic pwning
splendid uplifting).
Instead, it expanded to:
/bin /boot /challenge /dev /etc /flag /home /lib /lib32 /lib64 /libx32 /media /mnt /nix /opt /proc /root /run /sbin /srv /sys /tmp /usr /var
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run /p*
Your expansion did not expand to the requested files (happy optimistic pwning
splendid uplifting).
Instead, it expanded to:
/proc
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run /*p*
Error: your argument is too long! It must be 3 characters or less.
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run *p*
You got it! Here is your flag!
pwn.college{MtjTmD917H-tfR7vLWfpkua1vNB.0lM3kjNxwyM2EzNzEzW}
```
## Incorrect tangents I went on
Not able to get the right argument.
## What I learned
Learned how to use multiple * globs in an argument.
## References 
None 
