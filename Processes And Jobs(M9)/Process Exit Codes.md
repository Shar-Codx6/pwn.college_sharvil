# Process Exit Codes
In this challenge, you must retrieve the exit code returned by /challenge/get-code and then run /challenge/submit-code with that error code as an argument.
## My solve
**Flag:** `pwn.college{87vzxzpjZHYXclwWhPKH9J4LgHT.QX5YDO1wyM2EzNzEzW}`

```bash
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
47
hacker@processes~process-exit-codes:~$ /challenge/submit-code 47
CORRECT! Here is your flag:
pwn.college{87vzxzpjZHYXclwWhPKH9J4LgHT.QX5YDO1wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
I learned that if you dont specify $ with ?. It will always return 1.
## References 
None