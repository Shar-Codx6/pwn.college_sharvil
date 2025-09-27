# Matching with `*`
The challenge ask to start from your home directory, change your directory to /challenge, but use globbing to keep the argument you pass to cd to at most four characters! Once you're there, run /challenge/run for the flag!
## My solve
**Flag:** `pwn.college{YFj9l2q2rwyNVsi4n3Mi6gTWVO_.QXxIDO0wyM2EzNzEzW}`

```bash
hacker@globbing~matching-with-:~$ cd /ch*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{YFj9l2q2rwyNVsi4n3Mi6gTWVO_.QXxIDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
I was not able to figure out the `/ch*` in the starting.
## What I learned
I learned that * represents wildcard which changes the glob to any file which matches the pattern.
## References 
None