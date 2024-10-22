This module describes Linux File paths which is widely useful in knowing how files/directories are stored within.
The '/' indicates the root directory, where all the sub-directories and files branch out from.

## The Root
The filesystem always starts with the '/' indicating root directory from where all the directories and files can be further accessed/

## Absolute Paths
Absolute paths are directly invoked from the root directory. eg:- /dir1/dir2/myfile indicates that the file to be accessed is inside two nested directories.

## Positioning
The 'cd' command is widely used to help navigating inside a directory which means 'change directory'.

## Relative File Paths
The current working directory is crucial for relative paths but absolute paths are independent of the CWD.
  1. Relative File paths do not start with '/'.
  2. The CWD is where the prompt is currently located at
Every directory has two implicit enteries to refernce in paths - '.' and  '..'.
  The '.' indicates the same working directory that you are currently in.
  If the CWD is '/' then the relative and absolute paths are same.
**Giving naked paths is invalid in Linux as there might be same programs named with the same name as the system utilities.**


The "~" in the terminal indicates the user within the home directory (generally '/home/hacker').
Only the leading one is expanded whenever there is a nesting in the path.
**'cd' uses the home directory as the default destination.**
