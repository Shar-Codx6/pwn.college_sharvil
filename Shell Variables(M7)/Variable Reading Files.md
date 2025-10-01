# Variable Reading Files
use that to read /challenge/read_me into the PWN environment variable, and we'll give you the flag! The /challenge/read_me will keep changing, so you'll need to read it right into the PWN variable with one command!
## My solve
**Flag:** `pwn.college{Ai6KlNKIR5mghQssyiLpHOur6xd.QXwIDO0wyM2EzNzEzW}`

```bash
hacker@variables~reading-files:~$ read -p "INPUT: " PWN < /challenge/read_me
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{Ai6KlNKIR5mghQssyiLpHOur6xd.QXwIDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
I learned how to use the concept of redirecting Input and inputing variables.
## References 
None