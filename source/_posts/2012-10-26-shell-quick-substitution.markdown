---
layout: post
title: "Shell Quick Substitution"
date: 2012-10-26 09:17
comments: true
categories: SHELL
---

``` bash quick substitution
^string1^string2
```

If you find yourself needing to enter a very similar command multiple times this little command line trick that might save you some time.  This is really only helpful if your command line is somewhat long and repetitive. 

This is admittedly quite a contrived example but I think it gets the idea across:

``` bash example
scotmac:~ shewless$ ls file*.txt
file1.txt	file2.txt
scotmac:~ shewless$ for i in `cat file1.txt`; do echo $i; done
foo
bar
apple
scotmac:~ shewless$ ^file1^file2
for i in `cat file2.txt`; do echo $i; done
baz
qux
banana
scotmac:~ shewless$ 
```

Step by step:

- I have two files that I want to apply a similar action to:
``` bash list files
scotmac:~ shewless$ ls file*.txt
file1.txt	file2.txt
```
- I will run a command on file1.txt to list all of the lines in the file:
``` bash command on file1.txt
scotmac:~ shewless$ for i in `cat file1.txt`; do echo $i; done
foo
bar
apple
```
- I want to run the same command on file2.txt.  Note the **only** input I have provided is the first line.
``` bash command on file2.txt
scotmac:~ shewless$ ^file1^file2
for i in `cat file2.txt`; do echo $i; done
baz
qux
banana
```
Enjoy!
