### Thought Processes
Q1)
The ';' can be used to chain commands together instead of running them as separate lines.
In this challenge the /challenge/pwn must be chained with ; to /challenge/college to obtain flag.

Q2)
Create a file called x.sh and run two commands - /challenge/pwn and /challenge/college.
Invoke it in bash by passing the file name as an argument and obtain the flag.

Q3)
Create a script and store the commands /challenge/pwn and /challenge/college in it.
Then pipe the output using the '>' operator to another fille.
Concatenate the file and obtain the flag.

Q4)
Create a shell script called x.sh and run /challenge/solve in it.
Change the permissions of the file to make it executable using (chmod +x file_name).
Call it by its absolute path to invoke the function without using bash command and obtain the flag.
