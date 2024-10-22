### Thought Processes
Q1) 
In this question, the 'su' (switch user) command is being used. This then asks for the root password and checks whether permission has to be granted accordingly.
Since /challenge/get-root has SUID bit set, it can be accessed using su command and password is typed to obtain the flag accordingly.

Q2)
su is run and the argument 'zardus' is passed as a user to switch to 'zardus' user with the password being typed. Then /challenge/run is executed to obtain the flag.

Q3)
Since password are stored as encrypted texts. To decrypt them, a tool called John the Ripper can be used.
  john ./file_to_be_cracked
Here, zardus has an encrypted password, which has to be decrypted first, then su to Zardus and type in the password, and then run /challenge/run to obtain the flag.

Q4)
This challenge illustrates usage of 'sudo' (superuser do).
Sudo , instead of asking for a password, runs a command as root. This helps better for system administration without the threats of password being leaked.
use the sudo command to run /challenge/run and obtain the flag.
