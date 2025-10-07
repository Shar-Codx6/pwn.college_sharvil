# Deleting Newlines
 In this challenge, we'll inject a bunch of newlines into the flag. Delete them with tr's -d flag and the escaped newline specification!
## My solve
**Flag:** `pwn.college{ACu8uoqclvgtVJ4NSohcvrAlB73.0VNxEzNxwyM2EzNzEzW}`

```bash
hacker@data~deleting-newlines:~$ /challenge/run | tr -d '\n'
Your line-split flag: pwn.college{ACu8uoqclvgtVJ4NSohcvrAlB73.0VNxEzNxwyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
I learned how to delete new lines(\n).
## References 
None