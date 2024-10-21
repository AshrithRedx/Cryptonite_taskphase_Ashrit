This module teaches how the terminal a.k.a 'the shell' is used for programming and usage of variables within the shell.

> The echo command is used for printing out stuff in the standard output.

### The $ operator
The '$' operator is used to access the value within a variable. By default, the variable PWD holds the current working directory of the shell.

### The = operator
Like in any other programming language, the value is assigned to the variable with the '=' operator.
To assign a variable more than a single word, the value should be encapsulated within double quotes. (" ").

 To create a child shell we can use :
> sh
The variables created in the parent shell are not directly inherited to the child shell. They have to be **exported**.

### The env command
It is used for printing out every exported variable.

## Command Substitution
Used to directly store output of a command into a variable. This can be done via '$' operator.

## Reading User Input and Files
Storing input from the user can be done with the help of 'Read' command which takes input from the standard input..
Similarly, text can be stored within the variable using the read command and the '<' operator. 
