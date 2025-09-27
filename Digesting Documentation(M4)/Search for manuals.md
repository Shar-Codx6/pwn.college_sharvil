# Search for manuals
The challenge hides the manpage of /challenge by randomizing its name. To search for the manpage, first need to figure out the right manpage by doing `man man`. This will give the advanced usage of man command.
## My solve
**Flag:** `pwn.college{sAJNKr-fvwGGC_vzRn7f5dDUjDE.QX2EDO0wyM2EzNzEzW}`

```bash
hacker@man~searching-for-manuals:~$ man --regex flag
--Man-- next: linux32(1) [ view (return) | skip (Ctrl-D) | quit (Ctrl-C) ]
--Man-- next: pcap-config(1) [ view (return) | skip (Ctrl-D) | quit (Ctrl-C) ]
--Man-- next: srfvwvznfd(1) [ view (return) | skip (Ctrl-D) | quit (Ctrl-C) ]
^C
hacker@man~searching-for-manuals:~$ man --regex flag
--Man-- next: linux32(1) [ view (return) | skip (Ctrl-D) | quit (Ctrl-C) ]
--Man-- next: pcap-config(1) [ view (return) | skip (Ctrl-D) | quit (Ctrl-C) ]
--Man-- next: srfvwvznfd(1) [ view (return) | skip (Ctrl-D) | quit (Ctrl-C) ]
^C
hacker@man~searching-for-manuals:~$ /challenge/challenge --srfvwv 752
Correct usage! Your flag: pwn.college{sAJNKr-fvwGGC_vzRn7f5dDUjDE.QX2EDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
It was tough to figure out the hidden argument in the manpage.
## What I learned
I learned how to Search through the manpage and learned more about its usage.
## References 
None
