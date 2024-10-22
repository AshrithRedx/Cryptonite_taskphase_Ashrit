The permissions on any file or directory can be checked using 'ls -l' command.
+ if the beginning of the line is a 'd', it indicates that it is a directory.
+ if the beginning of the line is a '-', it indicates that it is a file.

  Further 9 characters are split into three groups of 3:
  1. The first three characters indicate the permissions of the owner.
  2. The next three characters indicate the permissions of the group.
  3. The last three characters indicate the permissions of all the other users/world.
 
  Two columns are present next to the list of permissions:
  1. First column indicates who the file is owned by.
  2. Second colunn indicates by which group the file is owned by.
 
  ### chown command
  chown (also known as CHANGE OWNER) command is used to change the owner of a particular file.
        chown [USER] [file]

  ### chgrp command
  chgrp (also known as CHANGE GROUP command is used to change the group which owns the file.
        chgrp [USER] [file]

  **The id command is useful for knowing the user and group ids incase they do not follow the default naming convention.**

  ### File Permissions:
  There are three types of file permissions:
  1.w - user/group/other can modify the files (or create/delete files in the directory)
  2. x - user/group/other can execute the file as a program (or can enter the directory, e.g., using `cd`)
  3. r - user/group/other can read the file (or list the directory)
  4- - nothing

  File permissions can be changed with the help of 'chmod' (CHANGE MODE) command.
          chmod WHO-/+WHAT
    where WHO stands for user/group/world
    where WHAT stands for r,w,x,s

  **File permissions can be entirely overwritten with the help of '=' command, different permissions can be assigned to different hosts simultaneously by separating them with ','.**

  **The SUID bit(s) can be assigned to a program to allow any user with executable permissions to run it without needing the permission of the host every single time.**
  
