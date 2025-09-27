# Mixing globs
Now, let's put the previous levels together! We put a few happy, but diversely-named files in /challenge/files. Go cd there and, using the globbing you've learned, write a single, short (6 characters or less) glob that (when passed as an argument to /challenge/run) will match the files "challenging", "educational", and "pwning"!
## My solve
**Flag:** `pwn.college{gHrSo111byf8hEkSvmwe5-yIJ3g.QX1IDO0wyM2EzNzEzW}`

```bash
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run /[cep]
Your expansion did not expand to the requested files (challenging, educational,
pwning). Instead, it expanded to:
/[cep]
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{gHrSo111byf8hEkSvmwe5-yIJ3g.QX1IDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
Mistyping [cep]* as [cep*]
## What I learned
Practicing arguments when used together.
## References 
None