

1. **Navigation**    
    - `ls`: List files and directories.
    - `cd [directory_name]`: Change directory.
    - `pwd`: Print the current working directory.

2. **File Management**    
    - `touch [filename]`: Create an empty file.
    - `cat [filename]`: Display the contents of a file.
    - `cp [file1] [file2]`: Copy a file.
    - `mv [file1] [file2]`: Move or rename a file.
    - `rm [filename]`: Delete a file or directory.
    - `grep [pattern] [filename]`: Searches for a pattern within files. [[Grep|more Info]]
    - `head [filename]``: Displays the first few lines of a file.
    - `tail [filename]``: Displays the last few lines of a file.
    - `less [filename]``: Views file contents with the ability to scroll.

3. **Directories**
    - `mkdir [directory_name]`: Create a directory (folder).
    - `rmdir [directory_name]`: Remove an empty directory.

4. **Permissions**    
    - `chmod [permissions] [filename]`: Change file permissions (read, write, execute).
    - `ls -l`: View detailed file information, including permissions.
    - ==`sudo [command}`==: Temporarily execute commands with the privileges of another user.

5. **Process Management**
- `ps [options]`: Lists running processes.
- `top [options]`: Provides a real-time view of running processes.
- `kill [signal] [PID]`: Sends a termination signal to a process. 

6. **Networking**
- `ping [ip]`: Tests connectivity to a host.
- `ifconfig`: Displays network interface information.

7. **System Information**
- `whoami`: Displays the currently logged-in username.
- `uname`: Prints basic system information.
- `free`: Shows memory usage.
- `df`: Shows disk space usage.

8. **Getting Help**
- **`man [command_name]`:** Brings up the manual page for a command for in-depth explanations.

9. **Network Tools**
- `netstat`: Shows network connections, routing tables, and interface statistics.
- `curl`: Transfers data to or from servers using various protocols (HTTP, FTP, etc.). Great for interacting with web APIs.
- `wget`: Downloads files non-interactively from the web. Useful for scripting.

10. **Utility**
- `find`: Searches for files based on various criteria (name, type, modification time, etc.).
- `rsync`: Efficiently synchronizes files and directories across local or remote systems.
- `ssh`: Securely logs into and executes commands on remote machines.

11. Package Management
- `apt-get update`: Refreshes the local list of available packages from the configured repositories
- `apt-get upgrade`: 
- `apt-get install`
- `apt-get remove`
- `apt-get autoremove`
- `apt-get search`

**==Important !!!==** 

**Text Editors**
- **vim:** A powerful and highly configurable text editor with a steep learning curve, but extremely efficient once mastered.
- **nano:** A simple, beginner-friendly text editor good for quick edits.
- **emacs:** Another powerful and extensible text editor, offering a vast array of features.

**Scripting**
- **bash:** The default shell on most Linux systems. Powerful for automation and scripting.
- **awk:** A pattern scanning and processing language excellent for text manipulation.
- **sed:** A stream editor used to perform transformations on text files.

