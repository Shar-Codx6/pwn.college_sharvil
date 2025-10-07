# Extracting Specific sections of text
In this challenge, the /challenge/run program will give you a bunch of lines with random numbers and single characters (characters of the flag) as columns. Use cut to extract the flag characters, then pipe them to tr -d "\n" (like the previous level!) to join them together into a single line.
## My solve
**Flag:** `pwn.college{QXY5TS-_ZN-5vEo4XbRzXfN_tlJ.01NxEzNxwyM2EzNzEzW}`

```bash
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run | cut -d " " -f 2 | tr -d "\n"
pwn.college{QXY5TS-_ZN-5vEo4XbRzXfN_tlJ.01NxEzNxwyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned
I first tried to check at what column I have to extract the text. Then I use the cut command to extract it and finally removing newline to get the final flag.
## References 
None