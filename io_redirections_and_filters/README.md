# Shell I/O Redirections and Filters

This project contains scripts that demonstrate basic shell I/O redirections and filters.

## Scripts

- `0-hello_world`: Prints "Hello, World" to the standard output.
- `1-confused_smiley`: Displays a confused smiley `"(Ôo)'"`.
- `2-hellofile`: Displays the content of the `/etc/passwd` file.
- `3-twofiles`: Displays the content of `/etc/passwd` and `/etc/hosts`.
- `4-lastlines`: Displays the last 10 lines of `/etc/passwd`.
- `5-firstlines`: Displays the first 10 lines of `/etc/passwd`.
- `1-confused_smiley`: Displays a confused smiley `"(Ôo)'"`.
- `2-hellofile`: Displays the content of the `/etc/passwd` file.
- `3-twofiles`: Displays the content of both `/etc/passwd` and `/etc/hosts`.
- `4-lastlines`: Displays the last 10 lines of the `/etc/passwd` file.
- `5-firstlines`: Displays the first 10 lines of the `/etc/passwd` file.
- `6-third_line`: Displays the third line of the file `iacta` using `head` and `tail`.
- `7-file`: Creates a file named `\*\\'"Best School"\'\\*$\?\*\*\*\*\*:)` containing the text "Best School".
## 8-cwd_state
This script runs the command `ls -la` and writes its output into a file named `ls_cwd_content`.

- If `ls_cwd_content` already exists, it will be overwritten.
- If `ls_cwd_content` does not exist, it will be created.
## 9-duplicate_last_line
This script duplicates the last line of the file `iacta` by appending it again at the end of the file using `tail -n 1` and `>>`.
## 10-no_more_js
This script deletes all regular files with a `.js` extension in the current directory and its subfolders using `find . -type f -name "*.js" -delete`. Directories are not affected.

