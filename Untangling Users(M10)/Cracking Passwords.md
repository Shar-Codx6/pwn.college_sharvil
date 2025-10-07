# Cracking Passwords
This level simulates this story, giving you a leak of /etc/shadow (in /challenge/shadow-leak). Crack it (this could take a few minutes), su to zardus, and run /challenge/run to get the flag
## My solve
**Flag:** `pwn.college{00uCwz0PLFpt4N051jtHJkZz3Pu.QX3UDN1wyM2EzNzEzW}`

```bash
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Created directory: /home/hacker/.john
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:21 100% 2/3 0.04631g/s 269.7p/s 269.7c/s 269.7C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{00uCwz0PLFpt4N051jtHJkZz3Pu.QX3UDN1wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned

## References 
None