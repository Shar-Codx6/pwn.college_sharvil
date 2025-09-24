# Hidden files
The challenge asks us to find the flag inside a hidden file in **/**.
## My solve
**Flag:** `pwn.college{spMJ3byz5ubRTKPBRYo9JhInjxB.QXwUDO0wyM2EzNzEzW}`

```bash
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls
bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv             bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-207101903830310  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ /dockerenv
bash: /dockerenv: No such file or directory
hacker@commands~hidden-files:/$ /.dockerenv
hacker@commands~hidden-files:/$ /.flag-207101903830310
bash: /.flag-207101903830310: Permission denied
hacker@commands~hidden-files:/$ cat /.flag-207101903830310
pwn.college{spMJ3byz5ubRTKPBRYo9JhInjxB.QXwUDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
I was not using `cat` while getting the flag.
## What I learned
I learned how to search hidden files in a file. Hidden files can only be made using .precended file.
## References 
None