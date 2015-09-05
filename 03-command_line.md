# Learn command line

Please follow and complete the free online [Command Line Crash Course
tutorial](http://cli.learncodethehardway.org/book/). This is a great,
quick tutorial. Each "chapter" focuses on a command. Type the commands
you see in the _Do This_ section, and read the _You Learned This_
section. Move on to the next chapter. You should be able to go through
these in a couple of hours.


---

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do, focused on things that are new, interesting, or otherwise worth remembering.

> > chmod -R [directory] 755 changes the permissions of directory and files within, -R means include directory's contents, chown <user>:<group> <file> changes the ownership of <file> to user and group, 

---


---

What does `ls` do? What do `ls -a`, `ls -l`, and `ls -lh` do? What combinations of those flags are meaningful?

> > ls lists information about files in the current directory.  -a stands for all and tells the command not to ignore files that start with a period, i.e. hidden files. -l stands for long listing format.  I use this to examine the permissions for the files in the directory. -lh does the same as -l but prints sizes in human readable format. You can use -la to list all files, including hidden files, in long format.  Yo

---


---

What does `xargs` do? Give an example of how to use it.

> > it takes what's in the stdin and executes echo command on it.  So, if you type simply xargs at the command prompt, it will wait for you to type something and echo it (after pressing Ctrl-D).  You can use it in a pipe, a la: echo 1 2 3 4 | xargs, which will output 1 2 3 4 to the console. The arguments to xargs expand the  functionality.  For instance, you can specify the delimiters with -d, limit the output per line with -n, prompt the user before executing with -p, or specify a command to execute other than the default echo command. For example, if you want to find all the C files that have the string stdlib.h in them, you would use the following command: find . -name '*.c' | xargs grep 'stdlib.h'.

---

