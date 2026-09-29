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
## 11-directories
This script counts the number of directories and subdirectories in the current directory, excluding `.` and `..`. Hidden directories are included in the count.
## 12-newest_files
This script displays the 10 newest files in the current directory, sorted from newest to oldest, using `ls -t | head -n 10`. Each file is shown on its own line.
## 13-unique
This script takes a list of words (one per line) and prints only those that appear exactly once. The output is sorted alphabetically, one word per line. It uses `sort | uniq -u`.
## 14-findthatword
This script displays all lines from `/etc/passwd` that contain the string `root` using `grep`.
## 15-countthatword
This script counts the number of lines in `/etc/passwd` that contain the string `bin` using `grep -c`.
## 16-whatsnext
This script displays all lines from `/etc/passwd` containing the string `root` and the three lines immediately following each match, using `grep -A 3`.
## 17-hidethisword
This script displays all lines from `/etc/passwd` that do not contain the string `bin` using `grep -v`.
## 18-letteronly
This script displays all lines in `/etc/ssh/sshd_config` that start with a letter (A–Z or a–z). It uses `grep '^[[:alpha:]]'` to filter out comments and non-letter lines.
## 19-AZ
This script replaces all characters `A` with `Z` and `c` with `e` from the input using `tr 'Ac' 'Ze'`.
## 20-hiago
This script removes all occurrences of the letters `c` and `C` from input using `tr -d 'cC'`.
## 21-reverse
This script reverses its input using the `rev` command. Each line of input is printed with its characters in reverse order.
## 22-users_and_homes
This script displays all users and their home directories from `/etc/passwd`, sorted alphabetically by username. It uses `cut -d: -f1,6 /etc/passwd | sort`.
