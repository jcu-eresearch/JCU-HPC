---
title: "Connecting to HPC"
teaching: 45
exercises: 0
questions:
- "How do I connect to HPC?"
- "How do I transfer files from my PC to HPC?"
objectives:
- "Learn to connect to HPC via `ssh` with a 'key' or password"
- "Learn to transfer files with `scp`, `rsync` & Filezilla"
- "Learn to stay connected with `screen`"
keypoints:
- "`ssh` allows us to connect securely to the HPC using keys or passwords"
- "We can transfer files to / from HPC in many ways, Filezilla operates on most platforms and has a simple GUI interface"
- "We can use `screen` to keep our interactive processes running"
- "When we connect we land on the 'login' node and see our home account"
---

Now it's time to take our hard-won UNIX knowledge to connect to the HPC using the program `ssh`. `ssh` stands for Secure Shell.
It's a method that we can use to not only connect to, but pass commands to, our HPC as well.
A basic `ssh` commands needs only the 'address' of the remote machine we're trying to connect to and the 'user' we're connecting as.

~~~
$ ssh [user]@[remote address]
~~~
{: .bash}

In our case, the user name is your 'JC' number and the address is 'zodiac.hpc.jcu.edu.au'.
So we can connect using

~~~
$ ssh jc152199@zodiac.hpc.jcu.edu.au
~~~
{: .bash}

Warnings & known hosts. Yes to proceed.
Enter password.

You are now connected to the HPC! How do I know this?  There are a few things we can check:
1) Your command prompt has changed (should now be user name & node you are connected to (29 or 30)
2) `ls` will show a new (and likely unfamiliar) file structure
3) `whoami` should prompt your JC number to appear on screen



 