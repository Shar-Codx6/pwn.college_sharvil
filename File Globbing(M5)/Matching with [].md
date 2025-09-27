# Matching with []
In this challenge, they placed a bunch of files in /challenge/files. Change your working directory to /challenge/files and run /challenge/run with a single argument that bracket-globs into file_b, file_a, file_s, and file_h!
## My solve
**Flag:** `pwn.college{k_y8t7C2kkN-Ct4iR-q1ny6uY8D.QXzIDO0wyM2EzNzEzW}`

```bash
hacker@globbing~matching-with-:~$ /challenge/file_[bash]
bash: /challenge/file_[bash]: No such file or directory
hacker@globbing~matching-with-:~$ ls /challenge/files
file_a  file_c  file_e  file_g  file_i  file_k  file_m  file_o  file_q  file_s  file_u  file_w  file_y
file_b  file_d  file_f  file_h  file_j  file_l  file_n  file_p  file_r  file_t  file_v  file_x  file_z
hacker@globbing~matching-with-:~$ cd /challenge/files
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[bash]
You got it! Here is your flag!
pwn.college{k_y8t7C2kkN-Ct4iR-q1ny6uY8D.QXzIDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
I learned how to [] argument.
## References 
None