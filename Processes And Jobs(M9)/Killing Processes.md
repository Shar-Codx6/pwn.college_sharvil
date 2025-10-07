# Killing processes
In this challenge, /challenge/run will refuse to run while /challenge/dont_run is running! You must find the dont_run process and kill it. If you fail, pwn.college will disavow all knowledge of your mission. 
## My solve
**Flag:** `pwn.college{helloworld}`

```bash
hacker@processes~killing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 13:52 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-init
root           7       1  0 13:52 ?        00:00:00 /run/dojo/bin/sleep 6h
root         135       1  0 13:52 ?        00:00:00 su -c /challenge/.launcher hacker
hacker       136     135  0 13:52 ?        00:00:00 /challenge/dont_run
hacker       137     136  0 13:52 ?        00:00:00 sleep 6h
hacker       163       1  0 13:52 ?        00:00:00 /nix/store/g0q8n7xfjp7znj41hcgrq893a9m0i474-ttyd-1.7.7/bin/ttyd --port 7
hacker       167     163  0 13:52 pts/1    00:00:00 /run/dojo/bin/bash --login
hacker       208       0  0 13:56 pts/0    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/bin/
hacker       214     208  0 13:56 pts/0    00:00:00 /run/dojo/bin/bash --login
hacker       223     214  0 13:56 pts/0    00:00:00 ps -ef
hacker@processes~killing-processes:~$ kill 136
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{sGsMCyvlD5fL2iYuCpnpbX-IZN4.QXyQDO0wyM2EzNzEzW}
```
## Incorrect tangents I went on
I first tried to list the processes using -e. In that I was not able to find the file /challenge/dont_run.
## What I learned
I ran ps -ef, with this I found the file /challenge/dont_run, I killed it and then ran /challenge/run to get the flag.
## References 
None