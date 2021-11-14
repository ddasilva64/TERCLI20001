# I-O redirections and control operators



```
command < file       -> redirects a command input to a file
command > file       -> redirects a command output of a file (be careful because overwrites the system)
command >> file      -> concatenates a command output to a file. If doesn't exist, creates it.
command 2> error.txt -> redirects a command error output to a file
command1 | command2  -> redirects command1 output with command2 input
command1; command2   -> runs consecutively
command1 & command2  -> runs asynchronously
command1 && command2 -> runs command2 only if command1 was executed successfully
command1 || command2 -> runs command1 or command2
```
