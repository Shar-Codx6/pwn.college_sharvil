# more cat practice
Challenge is same as previous where we find the flag inside the flag of another directory. 
## My solve
**Flag:** `pwn.college{sOi4CN65RNS3OC2TR8zhUIL6Abs.QXwITO0wyM2EzNzEzW}`

```bash
hacker@commands~more-catting-practice:~$ cat flag
cat: flag: No such file or directory
hacker@commands~more-catting-practice:~$ /usr/share/X11/flag
bash: /usr/share/X11/flag: Permission denied
hacker@commands~more-catting-practice:~$ cat /usr/share/X11/flag
pwn.college{sOi4CN65RNS3OC2TR8zhUIL6Abs.QXwITO0wyM2EzNzEzW}
hacker@commands~more-catting-practice:~$
```
## Incorrect tangents I went on
I first thought I might find a message by using command **cat flag**.
Then I tried to check the path of the flag.
Finally I realized instead of opening the path, I can read the file itself from **cat** command.
## What I learned
Learnt about using **cat** in opening files not in my home directory without using **cd** command.
## References 
None
