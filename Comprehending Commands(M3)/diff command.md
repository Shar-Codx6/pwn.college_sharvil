# Challenge Name
The challenge tells that, inside the folder **/challenge** there contains two files, both flags have 100 fake flags but the second file has the real flag. Use the diff command to find the real flag.
## My solve
**Flag:** `pwn.college{cl04C0zKjcIeYk-f7oiHv_q-pjt.01MwMDOxwyM2EzNzEzW}`

```bash
hacker@commands~comparing-files:~$ cd /challenge
hacker@commands~comparing-files:/challenge$ diff /decoys_only.txt /decoys_and_real.txt
diff: /decoys_only.txt: No such file or directory
diff: /decoys_and_real.txt: No such file or directory
hacker@commands~comparing-files:/challenge$ diff decoys_only.txt decoys_and_real.txt
8a9
> pwn.college{cl04C0zKjcIeYk-f7oiHv_q-pjt.01MwMDOxwyM2EzNzEzW}
```
## Incorrect tangents I went on
I used **/** in the first try because I thought I was suppose to take the path as well.
## What I learned
I learnt about the function of diff command and how it helps in finding difference in 2 similar files.

## References
none