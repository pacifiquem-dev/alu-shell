### 0-alias
Creates an alias `ls` that removes all files in the current directory.  
After sourcing the script, `ls` will delete files, while `\ls` bypasses the alias and lists files normally.
### 1-hello_you
Prints "hello" followed by the current Linux user.  
Uses the `$USER` environment variable to determine the username.
### 2-path
Appends `/action` to the end of the `$PATH` environment variable.  
After sourcing the script, the shell will look into `/action` last when searching for executables.
### 3-paths
Counts the number of directories in the `$PATH` environment variable.  
It splits `$PATH` by colons and counts each entry, including empty ones.
