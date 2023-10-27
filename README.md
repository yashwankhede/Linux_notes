# Linux_notes

# Linux Command Reference

This is a reference guide for various Linux commands and topics. Below, you'll find a list of commands and concepts related to Linux:

## Intro to Linux
- Linux is an open-source, Unix-like operating system.
- It is popular for its stability, security, and flexibility.
- Linux is widely used for servers, development, and embedded systems.
- Distributions like Ubuntu, CentOS, and Debian provide various versions of Linux.


## File Navigation, Creation, Absolute and Relative Paths
- The file system is organized as a tree structure with the root directory ("/").
- Use the "cd" command to change directories, and "pwd" to display the current directory.
- Absolute paths start from the root, e.g., "/home/user/documents".
- Relative paths are based on the current directory, e.g., "../folder/file".
- Change directory: `cd directory_path`
- Print working directory: `pwd`

## Copy and Move Files by Relative and Absolute Paths
- Use "cp" to copy files, e.g., "cp file.txt /destination/path".
- Use "mv" to move or rename files, e.g., "mv old.txt new.txt".
- Copy file: `cp source_file destination_path`
- Move or rename file: `mv source_file destination`

## bash_history and Alias
- "bash_history" is a file that stores your command history.
- "alias" allows you to create custom command shortcuts.
- View command history: `history`
- Create an alias: `alias alias_name='command'`

## Alias, Absolute and Relative Paths, Permanent Alias
- Example alias: "alias ll='ls -l'".
- To make aliases permanent, add them to "~/.bashrc" or "~/.bash_aliases" (for bash) or "~/.zshrc" (for zsh).
- To make an alias permanent, add it to `~/.bashrc`, `~/.bash_aliases`, or `~/.zshrc` using a text editor like `nano` or `vim`.

## cat, nano, vim, and Operators (>, >>, *)
- "cat" displays file content.
- "nano" is a simple text editor.
- "vim" is a powerful terminal text editor.
- Operators include ">" (redirect output), ">>" (append output), and "*" (wildcard for multiple files).
- Display file content: `cat filename`
- Edit a file with nano: `nano filename`
- Edit a file with vim: `vim filename`
- Redirection (output to file): `command > output_file`
- Append to a file: `command >> output_file`
- Use a wildcard: `*` (e.g., `ls *.txt`)

## File Permissions - Numeric (chmod)
- File permissions include Read (4), Write (2), Execute (1).
- Numeric representation, e.g., 644 (rw-r--r--).
- Change file permissions: `chmod 644 filename`

## File Permissions - Symbolic (chmod)
- Use symbolic representation, e.g., "chmod u+x file" (add execute permission to the user).
- Change file permissions symbolically: `chmod permissions filename`

## mkdir -p Flag
- "mkdir" creates directories, and "-p" flag creates parent directories if they don't exist.
- Create a directory and its parents if they don't exist: `mkdir -p path/to/new_directory`

## Basic Files Under "/"
- Important directories under "/" include "/bin," "/etc," "/home," "/usr," and "/var."
- These are standard directories and can be accessed using `cd /directory_name`.

## Environment Variables (bashrc, bash_logout, bash_history, profile, profile.d)
- Configuration files like "~/.bashrc" and "~/.bash_logout" control user settings.
- "~/.bash_history" stores command history.
- System-wide settings are in "/etc/profile" and "/etc/profile.d/."
- Edit user-specific environment settings: `nano ~/.bashrc`
- Edit system-wide environment settings: `sudo nano /etc/profile`

## Bash and Zsh Shell, Basic Shell Scripting
- Bash and Zsh are popular Unix shells.
- Shell scripting allows you to automate tasks by writing scripts with commands.
- No specific command, this involves writing shell scripts using text editors.

## Variables, How to Set Them (Where, Open, echo $SHELL, $PATH, $PS1)
- Environment variables are set in shell configuration files.
- Use "export" to make variables available to child processes.
- Common variables: "$SHELL" (current shell), "$PATH" (executable paths), "$PS1" (command prompt).
- Set a variable: `variable_name=value`
- View the value of a variable: `echo $variable_name`

## grep, egrep, Operators (|)
- "grep" searches for patterns in text.
- "egrep" is an extended version of "grep" supporting regular expressions.
- "|" (pipe) redirects output from one command to another.
- Search for a pattern in a file: `grep pattern filename`
- Extended grep (supports regular expressions): `egrep pattern filename`
- Pipe command output: `command1 | command2`

## User Management, adduser, deluser
- "adduser" adds new users.
- "deluser" removes users.
- "sudo" allows privileged operations for system administrators.
- Add a user: `adduser username`
- Remove a user: `deluser username`

These commands and concepts can be used in a Linux terminal for various tasks. Feel free to refer to this reference guide whenever needed.

Feel free to fork and contribute to this repository!
