# Epic filesystem quest
The challenge asks us to find the flag present in a file using commands like cd , ls and cat.
## My solve
**Flag:** `pwn.college{0EDW643bzAOYGbr358ufnylaclD.QX5IDO0wyM2EzNzEzW}`

```bash
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
ALERT  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin    challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat /flag
cat: /flag: Permission denied
hacker@commands~an-epic-filesystem-quest:/$ cat /ALERT
Yahaha, you found me!
The next clue is in: /usr/aarch64-linux-gnu/include/netatalk

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/aarch64-linux-gnu/include/netatalk/
MESSAGE-TRAPPED  at.h
hacker@commands~an-epic-filesystem-quest:/$ cat  /usr/aarch64-linux-gnu/include/netatalk/MESSAGE-TRAPPED
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/arch/arm/mach-qcom
hacker@commands~an-epic-filesystem-quest:/$ ls /opt/linux/linux-5.4/arch/arm/mach-qcom
CUE  Kconfig  Makefile  platsmp.c
hacker@commands~an-epic-filesystem-quest:/$ cat  /opt/linux/linux-5.4/arch/arm/mach-qcom/CUE
Yahaha, you found me!
The next clue is in: /usr/local/lib/python3.8/dist-packages/nbformat-5.10.4.dist-info
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/local/lib/python3.8/dist-packages/nbformat-5.10.4.dist-info/
INSIGHT  INSTALLER  METADATA  RECORD  WHEEL  entry_points.txt  licenses
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/local/lib/python3.8/dist-packages/nbformat-5.10.4.dist-info/entry_points.txt
[console_scripts]
jupyter-trust = nbformat.sign:TrustNotebookApp.launch_instance
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/local/lib/python3.8/dist-packages/nbformat-5.10.4.dist-info/INSIGHT
Great sleuthing!
The next clue is in: /usr/share/racket/pkgs/shell-completion

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/share/racket/pkgs/shell-completion/
LICENSE.txt  compiled  info.rkt  list-collects.rkt  racket-completion.bash  racket-completion.zsh
hacker@commands~an-epic-filesystem-quest:/$ ls -a  /usr/share/racket/pkgs/shell-completion/
.  ..  .MEMO  LICENSE.txt  compiled  info.rkt  list-collects.rkt  racket-completion.bash  racket-completion.zsh
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/share/racket/pkgs/shell-completion/.MEMO
Congratulations, you found the clue!
The next clue is in: /usr/share/racket/pkgs/racket-doc/syntax/scribblings
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/share/racket/pkgs/racket-
racket-cheat/ racket-doc/   racket-index/ racket-lib/
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/share/racket/pkgs/racket-doc/syntax/scribblings/
SPOILER                  flatten-begin.scrbl  macro-testing.scrbl   parse.scrbl                  syntax.scrbl
apply-transformer.scrbl  for-body.scrbl       modcode.scrbl         path-spec.scrbl              template.scrbl
boundmap.scrbl           for-transform.scrbl  modcollapse.scrbl     quote.scrbl                  to-string.scrbl
common.rkt               free-vars.scrbl      moddep.scrbl          reader-helpers.scrbl         toplevel.scrbl
compiled                 id-set.scrbl         modread.scrbl         readerr.scrbl                transformer-helpers.scrbl
context.scrbl            id-table.scrbl       modresolve.scrbl      srcloc.scrbl                 transformer.scrbl
contract.scrbl           info.rkt             module-helpers.scrbl  strip-context.scrbl          trusted-xforms.scrbl
datum.scrbl              intdef.scrbl         module-reader.scrbl   struct.scrbl                 wrap-modbeg.scrbl
define.scrbl             kerncase.scrbl       name.scrbl            stx.scrbl
docprovide.scrbl         keyword.scrbl        parse                 syntax-object-helpers.scrbl
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/share/racket/pkgs/racket-doc/syntax/scribblings/SPOILER
Lucky listing!
The next clue is in: /usr/local/lib/python3.8/dist-packages/jupyter_server/static/logo

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/local/lib/python3.8/dist-packages/jupyter_server/static/logo/
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/jupyter_server/static/logo$ ls
HINT  logo.png
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/jupyter_server/static/logo$ cat /HINT
cat: /HINT: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/jupyter_server/static/logo$ /HINT
bash: /HINT: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/jupyter_server/static/logo$ cat /logo.png
cat: /logo.png: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/jupyter_server/static/logo$ cd ~
hacker@commands~an-epic-filesystem-quest:~$ cat /logo.png
cat: /logo.png: No such file or directory
hacker@commands~an-epic-filesystem-quest:~$ /HINT
bash: /HINT: No such file or directory
hacker@commands~an-epic-filesystem-quest:~$ cat /usr/local/lib/python3.8/dist-packages/jupyter_server/static/logo/HINT
Great sleuthing!
The next clue is in: /usr/share/locale/es/LC_MESSAGES

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:~$ lt /usr/share/locale/es/LC_MESSAGES/
bash: lt: command not found
hacker@commands~an-epic-filesystem-quest:~$ ls /usr/share/locale/es/LC_MESSAGES/
BRIEF   dpkg.mo  iso_15924.mo   iso_3166-2.mo  iso_3166.mo    iso_4217.mo   iso_639-3.mo  iso_639_3.mo      nvim.mo
apt.mo  giac.mo  iso_3166-1.mo  iso_3166-3.mo  iso_3166_2.mo  iso_639-2.mo  iso_639.mo    libapt-pkg6.0.mo  sphinx.mo
hacker@commands~an-epic-filesystem-quest:~$ cat /usr/share/locale/es/LC_MESSAGES/BRIEF
cat: /usr/share/locale/es/LC_MESSAGES/BRIEF: Permission denied
hacker@commands~an-epic-filesystem-quest:~$ /usr/share/locale/es/LC_MESSAGES/BRIEF
bash: /usr/share/locale/es/LC_MESSAGES/BRIEF: Permission denied
hacker@commands~an-epic-filesystem-quest:~$ /usr/share/locale/es/LC_MESSAGES/
bash: /usr/share/locale/es/LC_MESSAGES/: Is a directory
hacker@commands~an-epic-filesystem-quest:~$ cd /usr/share/locale/es/LC_MESSAGES/
hacker@commands~an-epic-filesystem-quest:/usr/share/locale/es/LC_MESSAGES$ cat /BRIEF
cat: /BRIEF: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/share/locale/es/LC_MESSAGES$ cd ~
hacker@commands~an-epic-filesystem-quest:~$ cat /usr/share/locale/es/LC_MESSAGES/BRIEF
Yahaha, you found me!
The next clue is in: /usr/local/lib/python3.8/dist-packages/pip-25.0.1.dist-info

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:~$ ls -a /usr/local/lib/python3.8/dist-packages/pip-25.0.1.dist-info/
.  ..  .TIP  AUTHORS.txt  INSTALLER  LICENSE.txt  METADATA  RECORD  WHEEL  entry_points.txt  top_level.txt
hacker@commands~an-epic-filesystem-quest:~$ cat /usr/local/lib/python3.8/dist-packages/pip-25.0.1.dist-info/.TIP
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{0EDW643bzAOYGbr358ufnylaclD.QX5IDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
forgetting to change the directory when mentioned which let to errors.
## What I learned
Learned how useful the commands are when you are to search in a life directory with multiple files.
## References 
None