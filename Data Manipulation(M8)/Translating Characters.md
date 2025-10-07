# Translating Characters
In this level, /challenge/run will print the flag but will swap the casing of all characters (e.g., A will become a and vice-versa). 
## My solve
**Flag:** `pwn.college{w_QkB-jfW4YJrY8gxBvGKPv-NNm.01MxEzNxwyM2EzNzEzW}`

```bash
hacker@data~translating-characters:~$ /challenge/run | tr '[:upper:][:lower:]' '[:lower:][:upper:]'
yOUR CASE-SWAPPED FLAG:
pwn.college{w_QkB-jfW4YJrY8gxBvGKPv-NNm.01MxEzNxwyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
I learned how to change characters using the tr keyword.
## References 
None