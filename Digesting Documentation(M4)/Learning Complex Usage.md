# Learning complex usage
The challenge asks us to use the argument **--printfile** followed by another argument **/flag** which will print the flag. 
## My solve
**Flag:** `pwn.college{A3mUB7vE6eJfXO7AfJtmHoALnrK.QX1ITO0wyM2EzNzEzW}`

```bash
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /challenge/flag
Correct argument! Here is the /challenge/flag file:
cat: /challenge/flag: No such file or directory
hacker@man~learning-complex-usage:~$ /challenge/challenge
Incorrect usage! You must pass an argument to me (read the challenge
description for details).
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile
You must pass a file for --printfile to read!
hacker@man~learning-complex-usage:~$ /challenge/challenge --prntfile /flag
Incorrect usage! You passed the wrong argument (read the challenge description
for details).
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /flag
Correct argument! Here is the /flag file:
pwn.college{A3mUB7vE6eJfXO7AfJtmHoALnrK.QX1ITO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
I was not getting which location I had to add to print the file.
## What I learned
I learned about using a path in printing a complex program followed by its argument.
## References 
None