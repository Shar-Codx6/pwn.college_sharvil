# Moving files
This challenge wants you to move the **/flag** file into **/tmp/hack-the-planet** When you're done, run **/challenge/check**, which will check things out and give the flag to you.
## My solve
**Flag:** `pwn.college{Mxvn8qc7gnhtvzmgYdt6PY6Bwwt.0VOxEzNxwyM2EzNzEzW}`

```bash
hacker@commands~moving-files:~$ ls
 key   key.pub  '~'
hacker@commands~moving-files:~$ ls /flag
/flag
hacker@commands~moving-files:~$ cat /flag
cat: /flag: Permission denied
hacker@commands~moving-files:~$ ls /tmp/hack-the-planet
ls: cannot access '/tmp/hack-the-planet': No such file or directory
hacker@commands~moving-files:~$ mv /flag /tmp/hack-the-planet
Correct! Performing 'mv /flag /tmp/hack-the-planet'.
hacker@commands~moving-files:~$ /challenge/check
Congrats! You successfully moved the flag to /tmp/hack-the-planet! Here it is:
pwn.college{Mxvn8qc7gnhtvzmgYdt6PY6Bwwt.0VOxEzNxwyM2EzNzEzW}
```
## Incorrect tangents I went on
I first tried to check the contents in the two files given. The files were restricted.
## What I learned
I learned how to move file content from one file to another.
## References 
None
