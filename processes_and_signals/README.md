### 0-what-is-my-pid
- **Location:** `processes_and_signals/0-what-is-my-pid`
- **Description:** Displays the PID (Process ID) of the script itself.
- **Usage:**
  ```bash
  ./0-what-is-my-pid
### 1-list_your_processes
- **Location:** `processes_and_signals/1-list_your_processes`
- **Description:** Displays a list of currently running processes for all users in a user-oriented format, showing the process hierarchy.
- **Usage:**
  ```bash
  ./1-list_your_processes | head -50
### 2-show_your_bash_pid
- **Location:** `processes_and_signals/2-show_your_bash_pid`
- **Description:** Displays lines containing the word "bash" from the process list, allowing you to easily identify the PID of your Bash process.  
- **Notes:** The third line of the script includes `# shellcheck disable=SC2009` to suppress warnings about using `ps | grep` instead of `pgrep`, as required by the project instructions.
- **Usage:**
  ```bash
  ./2-show_your_bash_pid


