
# Git Shell Commands Note 
---
## ✨Git 
![](https://git-scm.com/images/logo@2x.png)
Git is a distributed version management system for tracking changes in computer files
and coordinating the operations of those files among multiple users.
Software development is primarily used for source code management, 
but can be used to continuously track changes in any set of files.
---
## ⌨Commonds

### I/O Redirection : Standard Output

- '>' : create and save the output in a file ( Overwrite existing content. )
- '>>' : appends output to an extising file ( if it already exitsts ) or create and write to a new file if it doesn't exist.
- cat : displays the content of a text file.

### Change permissions
- chmod : changes permissions.
    - chomd 600 some_file ( 6 = 110 rw- , 0 = 000 ---, 0 = 000 --- )
    - rwx = 7, rw- = 6, r-x = 5, r-- = 4

### Create shell script
- text editors script .sh
    - text editors : vi, vim | Emacs | nano | gedit | kwrite etc..
    - [Ctrl] + character : script commands

### History
- history : see previous command history

### Convenience
- [\\] : ignore line change in command ("enter"), to enter a long command in multiple lines.

---
## 🗎Details
- Pipelines "|" : feeds output of previous command to input of next command.
    - ex) command 1 | command 2 | commnad 3 | ...
- Expansion : Special characters expand its meaning when given to shell commands.
    - \* : All Files
    - \~ : Directory of the current user
- Permissions : Files and directories have a permission assigned differently to owner / group / others.
![](https://linuxcommand.org/images/file_permissions.png)
    - r : read
    - w : write
    - x : execute
- Superuser : all system administation authority
---

