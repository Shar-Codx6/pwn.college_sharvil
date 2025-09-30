# Filtering with grep -v
In this challenge, /challenge/run will output the flag to stdout, but it will also output over 1000 decoy flags (containing the word DECOY somewhere in the flag) mixed in with the real flag. You'll need to filter out the decoys while keeping the real flag!
## My solve
**Flag:** `pwn.college{ElbI6tWSGDO072Uo9wx_gBenJSH.0FOxEzNxwyM2EzNzEzW}`

```bash
hacker@piping~filtering-with-grep-v:~$ /challenge/run | grep -v DECOY
pwn.college{ElbI6tWSGDO072Uo9wx_gBenJSH.0FOxEzNxwyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
I learned the usage of grep -v.
## References 
None