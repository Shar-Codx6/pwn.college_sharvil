# Extracting first lines with head
This challenge's /challenge/pwn outputs a bunch of data, and you'll need to pipe it through head to grab just the first 7 lines and then pipe them onwards to /challenge/college, which will give you the flag.
## My solve
**Flag:** `pwn.college{wnElNDQ1t76u4oM_uOd9j5H6TIc.0lNxEzNxwyM2EzNzEzW}`

type in your solve and your thought process behind solving the challenge. Include as much as info as possible. Use triple ticks for bash.
```bash
hacker@data~extracting-the-first-lines-with-head:~$ /challenge/pwn | head -n 7 | /challenge/college
Congratulations, you piped the right codes!
pwn.college{wnElNDQ1t76u4oM_uOd9j5H6TIc.0lNxEzNxwyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
I learned how head command works.
## References 
None