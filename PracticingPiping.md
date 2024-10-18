This module gives insights about input and output redirection. Linux has three channels of communication:
  1. Standard Input through which process taakes input. ALso known as stdin.
  2. Standard Output through which process outputs data. Also known as stdout.
  3. Standard Error where process outputs error detaiils. Also known as stderr.

 ## Redirecting and Appending Output
 Standard output can be redirected to any particular file using the '>' operator.
 To append the output of a second file onto already existing file with data, the '>>' operator can be used, If only '>' is used, this will lead to overwriting of previous data.


A File Descriptor (FD) is a number that describes the communication channel.
  1. FD 0: Standard Input
  2. FD 1 : Standard Output
  3. FD 2 : Standard Error


 ## Redirecting Input and Errors
 For redirecting errors, the FD number has to be put before the '>' operator('2>'). 
 By default it is '1>' indicating standard output.
 Redirecting input to programs can be done with the '<' operator, with destination on the left, and the source on the right.
 The 'rev' command is used to reverse and store the input in the file.


The output can directly be formatted with the 'grep'  command after the piping operator(|) to eliminate the need to store the output.
The standard output from the left hand side only will be availabe and connected to the standard input of the right hand side of the operator.

**The shell has a >& operator, which redirects a file descriptor to another. This happens in a two-step process.**

The 'tee' command is used to retain the original output even after the piping operation.
When using process substitution, a temporary named pipe is created, allowing data to be passed to commands that read from standard input.
