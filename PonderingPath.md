### Thought Processes
Q1)
In this challenge, the PATH must be set to ' ' i.e, path must be erased so that bash does not find the rm command.
Run /challenge/run and obtain the output.

Q2)
Set /challenge/run to the PATH where the win command lies.
Invoke /challenge/run so that win command gets executed and obtain the flag.

Q3)
Create a shell script called win and place a command to cat /flag within it.
Now, note the location of the win script (preferably in the home directory) and add it to PATH variable.
Obtain the current PATH using 'echo $PATH' where the cat command will be present in one of the many directories.
Chain the paths using the ';' command where the with both the path of the win file and original path are present.
Run /challenge/run and since it can read the win shell, obtain the flag.

Q4)
Create a win shell again and store cat /flag in it.
Find the location of the win file and chain it with the original path in the PATH variable using the ';' operator.
Run /challenge run and obtain the flag.
