# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > 

pwd 

mkdir

rmdir

ls

ls -a

cp

touch 

rm 

echo 

cd 

which

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> > 
'ls' - list of files in directory

'ls -a' - shows hidden files as well

'ls -l' - shows file information as well as the permissions given

'ls -lh' - shows files that human readable format

'ls -lah'

'ls -t' - sorts files by modification time




### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > 

ls -a : I would like to see all files

ls -t : Newest files should be seen first

ls -d : Sometimes it is convenient to just see directories

ls -l : Useful to see all information '

ls -x : Improves readability 

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > Example

'xargs' converts input from standard input into a command.

Ex: xargs effectively finds file names
xargs -l find -name



