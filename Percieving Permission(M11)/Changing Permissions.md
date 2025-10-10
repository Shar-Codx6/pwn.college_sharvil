# Changing Permissions
In this challenge, you must change the permissions of the /flag file to read it! Typically, you need to have write access to the file in order to change its permissions, but I have made the chmod command all-powerful for this level, and you can chmod anything you want even though you are the hacker user. This is an ultimate power. The /flag file is owned by root, and you can't change that, but you can make it readable. Go and solve this!
## My solve
**Flag:** `pwn.college{Ec5w4L26iTPdHwhOEGDaeHGICUT.QXzcjM1wyM2EzNzEzW}`

```bash
hacker@permissions~changing-permissions:~$ chmod a+rwx /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{Ec5w4L26iTPdHwhOEGDaeHGICUT.QXzcjM1wyM2EzNzEzW}
```
## Incorrect tangents I went on
None
## What I learned

## References 
None