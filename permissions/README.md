# shell permissions
This folder contains scripts related to shell permissions
## Scripts
- '0-iam_betty': Switches the current user to the user 'betty'.
- '1-who_am_i': Prints the effective username of the current user.
- '2-groups': Prints all the groups the current user belongs to.
- '3-new_owner': Changes the owner of the file 'hello' to the user 'betty'.
- '4-empty': Creates an empty file named `hello`.
- `5-execute`: Adds execute permission to the file `hello` for the owner.
- `6-multiple_permissions`: Adds execute permission to the owner and group, and read permission to others for the file `hello`.
- `7-everybody`: Adds execute permission to the owner, group, and others for the file `hello`.
- `8-James_Bond`: Sets permissions so owner and group have none, while others have full (read, write, execute) access to `hello`.
