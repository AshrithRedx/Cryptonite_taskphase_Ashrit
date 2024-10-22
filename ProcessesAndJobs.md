#### In Linux- software is split into two categories
1. Operating System Kernels
2. Processes

### Processes
The processes can be listed out using the 'ps' command, in short for process status.
The ps commad lists out few coumns by default:
1. The PID, used to indicate the ID of the process.
2. The TTY, used to incdicate terminal being used.
3. The TIME, used to indicate CPU time taken to execute the process.

+ 'ps' , by itself is not very useful, so additional arguments may have to be passed.

#### ps-ef argument
The e stands for **every process** and f stands for **full format**, which can be combined into a single argument -ef.

#### ps aux argument
The a stands for **all users**, u stands for **user-readable input** and x to **list processes not running in the terminal**.

These both commands can be used to gain more information about the processes running.

#### Terminate/Kill Processes
We have previously seen the usage of 'sleep' command which puts the process to sleep for a specified amount of time. Likewise, we can use the 'kill' command to terminate a process entirely.



## Thought Processes
### Question 1
Since the question removed the usage of 'ls' to find /challenge directory, we have to list out the processes using ps -ef or ps aux and search for the running processes to find the flag.

### Question 2
In this question, the /challenge/dont-run has to be terminated using the 'kill' command and run /challenge/run to obtain the flag. The PID has to be passed of the /challenge/dont-kill as an argument to kill command.

### Question 3
> Ctrl+ C
This is used to interrupt an ongoing process, and cleanly exits the process. Simply put Ctrl + C to interrupt the /challenge/run process.

### Question 4
> Ctrl + Z
This is used to suspend the processes to the background. Simply put Ctrl + Z to put the running 'run' to the background and execute run once more to create a copy of the process.

### Question 5
Run the 'run' program, suspend it using Ctrl + Z and then resume it to the foreground using the 'fg' command.

### Question 6
Similarly, the suspended programs can be launched in the background too using the 'bg' command. Suspend and run the 'run' command in the background.

### Question 7
Run the 'fg' command to foreground all the processes running in the background.

### Question 8
/challenge/run should be running in the background without needing to suspend it. This can be done by simply concatenating the '&' at the end of the command line.

### Question 9
Obtain the exit code of /challenge/get-code using the '$?' operators. **0 indicates if the command ran successfully and 1 indicates that command ran unsuccessfully.**
Obtain the exit code and run /challenge/submit-code with the code obtained as an argument.
