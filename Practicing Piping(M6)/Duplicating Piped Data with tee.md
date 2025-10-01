# Challenge Name
This process' /challenge/pwn must be piped into /challenge/college, but you'll need to intercept the data to see what pwn needs from you!
## My solve
**Flag:** `pwn.college{Mxqm7Y-D9Zffq2U1Q8JOXcu6oTY.QXxITO0wyM2EzNzEzW}`

```bash
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee output | /challenge/college
Processing...
WARNING: you are overwriting file output with tee's output...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat output'
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "Mxqm7Y-D"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret Mxqm7Y-D | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
/Great job! Here is your flag:
pwn.college{Mxqm7Y-D9Zffq2U1Q8JOXcu6oTY.QXxITO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
I was not able to able to understand how to duplicate in the first try. It took me multiple attempts to recognise the challenge.
## What I learned
I learned that first we duplicate the output of /challenge/pwn into an output file using tee command. After using cat to view the output file, we then use the secret code to get the flag.
## References 
None