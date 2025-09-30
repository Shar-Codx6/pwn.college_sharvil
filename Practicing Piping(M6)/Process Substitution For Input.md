# Process Substitution For Input
Now for your challenge! Recall what you learned in the diff challenge from Comprehending Commands. In that challenge, you diffed two files. Now, you'll diff two sets of command outputs: /challenge/print_decoys, which will print a bunch of decoy flags, and /challenge/print_decoys_and_flag which will print those same decoys plus the real flag.
Use process substitution with diff to compare the outputs of these two programs and find your flag!
## My solve
**Flag:** `pwn.college{cGa7OdJrMuerhOPzdb5n4dkLEu3.0lNwMDOxwyM2EzNzEzW}`

```bash
hacker@piping~process-substitution-for-input:~$ diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
99a100
> pwn.college{cGa7OdJrMuerhOPzdb5n4dkLEu3.0lNwMDOxwyM2EzNzEzW}
```
## Incorrect tangents I went on
I was trying to fit two commands in one bracket which was incorrect.
## What I learned
I learned how to use the substitution process to perform commands using files.
## References 
None