# Listing files
The challenge asks us to find the file by listing the files in **/challenge**.
## My solve
**Flag:** `pwn.college{0rm-_qmSJRnvZxselx8NIYyJyqZ.QX4IDO0wyM2EzNzEzW}`

```bash
hacker@commands~listing-files:~$ ls /challenge
25694-renamed-run-31255  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/25694-renamed-run-31255
Yahaha, you found me! Here is your flag:
pwn.college{0rm-_qmSJRnvZxselx8NIYyJyqZ.QX4IDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
I was trying to `cat` the `/25694-renamed-run-31255` file which was not allowing me to get the flag.
## What I learned
I learnt that after listing the files, I can just execute the file to see the output.
## References 
None
