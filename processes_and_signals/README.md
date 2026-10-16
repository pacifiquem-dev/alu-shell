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
### 3-show_your_bash_pid_made_easy
- **Location:** `processes_and_signals/3-show_your_bash_pid_made_easy`
- **Description:** Displays the PID and process name of processes whose name contains "bash". Uses the `/proc` filesystem instead of `ps`.
- **Usage:**
  ```bash
  ./3-show_your_bash_pid_made_easy
### 4-to_infinity_and_beyond
- **Location:** `processes_and_signals/4-to_infinity_and_beyond`
- **Description:** Displays "To infinity and beyond" indefinitely, with a 2-second pause between each iteration.
- **Usage:**
  ```bash
  ./4-to_infinity_and_beyond
### 5-dont_stop_me_now
- **Location:** `processes_and_signals/5-dont_stop_me_now`
- **Description:** Stops the `4-to_infinity_and_beyond` process using `kill`.
- **Usage:**
### 6-stop_me_if_you_can
- **Location:** `processes_and_signals/6-stop_me_if_you_can`
- **Description:** Stops the `4-to_infinity_and_beyond` process without using `kill` or `killall`. Uses the `/proc` filesystem to send a termination signal.
### 7-highlander
- **Location:** `processes_and_signals/7-highlander`
- **Description:** Displays "To infinity and beyond" indefinitely, with a 2-second pause. Prints "I am invincible!!!" when receiving a SIGTERM signal.
### 8-beheaded_process
- **Location:** `processes_and_signals/8-beheaded_process`
- **Description:** Kills the `7-highlander` process by sending a `SIGKILL` signal using `pkill`.
### 10-process_and_pid_file
- **Location:** `processes_and_signals/10-process_and_pid_file`
- **Description:** Creates `/var/run/myscript.pid` containing its PID. Displays "To infinity and beyond" indefinitely. Handles signals:
  - **SIGTERM:** Prints "I hate the kill command", deletes the PID file, and terminates.
  - **SIGINT:** Prints "Y U no love me?!".
  - **SIGQUIT:** Deletes the PID file and terminates.
### manage_my_process
- **Location:** `processes_and_signals/manage_my_process`
- **Description:** Writes "I am alive!" to `/tmp/my_process` indefinitely, pausing 2 seconds between each message.

### 11-manage_my_process
- **Location:** `processes_and_signals/11-manage_my_process`
- **Description:** Init-style script to manage `manage_my_process`. Supports start, stop, and restart commands.

