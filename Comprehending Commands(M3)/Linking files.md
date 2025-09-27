# Linking files
The challenge asks us to link the file `/home/hacker/not-the-flag` to `/flag` and then execute `/challenge/catflag`
## My solve
**Flag:** `pwn.college{cfQVO3tdHOQvP4hE-bAdgAjayQs.QX5ETN1wyM2EzNzEzW}`

```bash
hacker@commands~linking-files:~$ ln -s /flag ~/not-the-flag
hacker@commands~linking-files:~$ /challenge/flag
bash: /challenge/flag: No such file or directory
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{cfQVO3tdHOQvP4hE-bAdgAjayQs.QX5ETN1wyM2EzNzEzW}
```
## Incorrect tangents I went on
I by mistakely linked `ln -s ~/not-the-flag /challenge/catflag`. Because of this I was not able to link **not-the-flag** file to the main flag file. I had to unlink not-the-flag file and link it to /flag.
## What I learned
I learned about the process of linking files where the linked files basically stores the address of the original.
## References 
None 