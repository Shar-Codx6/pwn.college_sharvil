# Matching paths with []
The challenge has bunch of files in /challenge/files. Starting from your home directory, run /challenge/run with a single argument that bracket-globs into the absolute paths to the file_b, file_a, file_s, and file_h files.

## My solve
**Flag:** `pwn.college{osvTlzgeYa0nA6rYIW8fpwaNSgW.QX0IDO0wyM2EzNzEzW}`

type in your solve and your thought process behind solving the challenge. Include as much as info as possible. Use triple ticks for bash.
```bash
hacker@globbing~matching-paths-with-:~$ /challenge/run
Error: you did not use a square bracket glob...
hacker@globbing~matching-paths-with-:~$ /challenge/run file_[bash]
Error: you will need to specify the path to the files as part of your glob
argument, since they are in a different directory than your current working
directory!
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/file_[bash]
Error: you will need to specify the path to the files as part of your glob
argument, since they are in a different directory than your current working
directory!
HINT: You are trying to specify files in the /challenge directory, but the
files are actually in the /challenge/files directory.
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[bash]
You got it! Here is your flag!
pwn.college{osvTlzgeYa0nA6rYIW8fpwaNSgW.QX0IDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
Not using the absolute path when using the [] glob.
## What I learned
I learned how to use [] using absolute path.
## References 
None