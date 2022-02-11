# Copy Whole Directories with `scp -r`
by Bryan Budiputra, CSE15L

Using the command `ls`, we can see the all the files in the local machine.

![Image](images/localDir.png)

Now we want to copy the whole markdown-parse directory to the ieng6 account. To do this, we can use the following command:

```scp -r . cs15lwi22@ieng6.ucsd.edu:~/markdown-parse```

![Image](images/scpr1.png)

![Image](images/scpr2.png)

To show this works, we will compile and run the files in the remote server.

![Image](images/runOnIeng6.png)

We have successfully copied a whole directory to a remote server!

However, we can still optimize this system by using only one command-line to do all of the above.

We can write a command in quotes at the end of an `ssh` command to directly run it on the remote server, then exit. We can also use semicolons to run multiple commands on the same line. Combining both of these, we can do the following:

![Image](images/oneline1.png)

![Image](images/oneline2.png)