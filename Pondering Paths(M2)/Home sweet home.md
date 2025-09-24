# Home Sweet Home
In this challenge, **/challenge/run** will write a copy of the flag to any file you specified as an argument under this constraints:
1. Your argument must be an absolute path.
2. The path must be inside your home directory.
3. Before expansion, your argument must be three characters or less.
## My solve
**Flag:** `pwn.college{helloworld}`

```bash
hacker@paths~home-sweet-home:~$ /challenge/run ~/~
Writing the file to /home/hacker/~!
... and reading it back to you:
```

## What I learned
I learned that /home/hacker has a shorthand which is ~ and I was able to get the flag by commanding to the given path.