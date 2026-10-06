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
### 4-global_variables
Lists all environment variables currently defined in the shell using the `printenv` command.
### 5-local_variables
Lists all local variables, environment variables, and functions using the `set` command.
### 6-create_local_variable
Creates a local variable named `BEST` with the value `School`.  
This variable is only available in the current shell session unless exported.
### 7-create_global_variable
Creates a global environment variable named `BEST` with the value `School`.  
This variable is exported, so it is available to child processes and other programs.
### 8-true_knowledge
Prints the result of adding 128 to the value stored in the environment variable `TRUEKNOWLEDGE`.  
Uses Bash arithmetic expansion: `echo $((TRUEKNOWLEDGE + 128))`.
### 9-divide_and_rule
Prints the result of dividing the environment variable `POWER` by `DIVIDE`.  
Uses Bash arithmetic expansion: `echo $((POWER / DIVIDE))`.
### 10-love_exponent_breath
Displays the result of raising the environment variable `BREATH` to the power of `LOVE`.  
Uses Bash arithmetic expansion: `echo $((BREATH ** LOVE))`.
### 11-binary_to_decimal
Converts a binary number stored in the environment variable `BINARY` into decimal.  
Uses Bash arithmetic expansion with base notation: `echo $((2#$BINARY))`.
### 12-combinations
Prints all possible two-letter lowercase combinations from `aa` to `zz`, excluding `oo`.  
One combination per line, alpha ordered. Script length ≤ 64 characters.
