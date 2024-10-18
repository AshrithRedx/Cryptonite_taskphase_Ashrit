This module further elaborates on the usage of commands in the shell. The most popular commands being:
  1. echo
  2. cat
  3. grep
  4. ls
  5. touch
  6. rm
  7. mkdir
  8. find

### Cat
The 'cat' comand is used for reading out/concatenating the files with one mor more arguments. If no arguments are provided, then cat reads from standard I/O and O/P.
cat even accepts absolute paths as an argument.

### grep
The 'grep' command is used to search a file for a particular string after specifiying the path of the file.

### ls
The 'ls' command is used to list all the files/directories in the CWD when no arguments are passed and same when a directory is passed as an argument.
The hidden files can be listed out by passing '-a' as an argument, indicating all the files to be listed out (hidden and non-hidden).

### touch
The 'touch' command is used to create new files in the CWD.

### rm
The 'rm' command is used to delete exisitng file in the CWD(if any).

### mkdir
A new directory can be created within the CWD using the 'mkdir' command.

### find
The 'find' command works as a recursive function from the CWD and matches every file.
It can be used by passing '-name' as a parameter along with the file name. 

## Linking in Linux
Linux uses two types of links:  
  1. Hard Link: Provide Multiple addresses for same data, but comes with downsides.
  2. Soft Link: Contain Reference to the Original File name, functioning like a forwarding device. Also called as symlinks.
'Ln -s' can be used to create a symlink to the original file.
**The 'file' command detects the type of the file mentioned. It will detect whether any file is a symlink to the original file.**
