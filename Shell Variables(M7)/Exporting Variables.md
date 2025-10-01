# Exporting Variables
In this challenge, you must invoke /challenge/run with the PWN variable exported and set to the value COLLEGE, and the COLLEGE variable set to the value PWN but not exported.
## My solve
**Flag:** `pwn.college{Egn6BOnAIGjmd7Bhx-1IrrPFr1v.QXyYTN0wyM2EzNzEzW}`

```bash
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ sh
sh-5.2$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{Egn6BOnAIGjmd7Bhx-1IrrPFr1v.QXyYTN0wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
Exporting variables lets us use them in a child shell.
## References 
None