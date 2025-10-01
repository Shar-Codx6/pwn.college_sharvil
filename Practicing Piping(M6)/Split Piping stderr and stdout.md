# Split Piping stdrr and stdout
In this challenge, you have:
1. /challenge/hack: this produces data on stdout and stderr
2. /challenge/the: you must redirect hack's stderr to this program
3. /challenge/planet: you must redirect hack's stdout to this program
Go get the flag!
## My solve
**Flag:** `pwn.college{A1egLjIh5rzkR69kQQywUY8Riyk.QXxQDM2wyM2EzNzEzW}`

type in your solve and your thought process behind solving the challenge. Include as much as info as possible. Use triple ticks for bash.
```bash
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hacker 2> >(/challenge/the) > >(/challenge/planet)
hacker@piping~split-piping-stderr-and-stdout:~$ You are redirecting standard error *of /challenge/planet*! Instead, you must
redirect standard error of 'hack'. This must be done *before* any |. The right
side of the pipe is a different command, with its own redirection, than the
left side!
Are you sure you're properly redirecting /challenge/hack's standard error into
'/challenge/the'?
/challenge/hacker 2> >(/challenge/the) > >(/chal
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack > >( /challenge/planet ) 2> >( /challenge/the )
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{A1egLjIh5rzkR69kQQywUY8Riyk.QXxQDM2wyM2EzNzEzW}
```
## Incorrect tangents I went on
I was redirecting the stderr file to the stdout file(/challenge/planet).
## What I learned
I learned how to split the error and the output from a program and store it in 2 seperate files.
## References 
None