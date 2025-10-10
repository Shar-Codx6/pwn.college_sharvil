# Executable files
In this challenge, the /challenge/run program will give you the flag, but you must first make it executable! Remember your chmod, and get /challenge/run to tell you the flag!
## My solve
**Flag:** `pwn.college{helloworld}`

```bash
hacker@permissions~executable-files:~$ ls -l /challenge/run
-r--r--r-- 1 hacker hacker 32 Jan 14  2025 /challenge/run
hacker@permissions~executable-files:~$ chmod o+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/r
bash: /challenge/r: No such file or directory
hacker@permissions~executable-files:~$ /challenge/run
bash: /challenge/run: Permission denied
hacker@permissions~executable-files:~$ chmod o+x /challenge/run
hacker@permissions~executable-files:~$ ls -l /challenge/run
-r--r--r-x 1 hacker hacker 32 Jan 14  2025 /challenge/run
hacker@permissions~executable-files:~$ chmod u+wx /challenge/run
hacker@permissions~executable-files:~$ ls -l /challenge/run
-rwxr--r-x 1 hacker hacker 32 Jan 14  2025 /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
Successful execution! Here is your flag:
pwn.college{k8I224wcu8A8MR36ZPH0mCxVuL7.QXyEjN0wyM2EzNzEzW}
```
## Incorrect tangents I went on
I thought the file will count in other group, then I realized that the executable part is not present in the user part itself.
## What I learned

## References 
None