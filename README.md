
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

### Directory

- pwd : shows the current path in a hierarchical directory
- cd : change directory
    - cd path : Move to the designated path
- ls : list files and directories
    - /bin : List the files in the /bin diretory
    - -l : List the files in the working directory in long format
    - -l /etc /bin : List the fiels in the /bin and /etc directory in long format
    - -la : List all files (Including normally hidden files)

### Manipulation
- cp : copt files and directories
    - file 1 file 2 : copies the contents of file 1 into file 2 / does not exist, it is created
    - -i file 1 file 2 : if file 2 exists, the user is prompted before it is overwritten with the contents of file 1
    - file dir : copy the contents of file1 inside of directory dir.
    - -R dir1 dir2 : copy the contents of the directory dir1. / directory dir2 does not exist, it is created
- mv : move files and directories or rename them
    - file 1 file 2 : If file 2 does not exist, then file 1 is renamed file 2 But If file 2 exists, it contents are replaced with the contents of file 1
    - -i file 1 file 2 : if file 2 exists, the user is prompted before it is overwritten with the contents of file 1
    - file 1 file 2 dir : The files file 1 and file 2 are moved to dir / dir does not exist, it will exit with an error
    - dir 1 dir 2 : If dir2 does not exist, then dir 1 is renamed dir2 / dir 2 exists, the dir 1 is moved within dir 2
- rm : delete files and directories permantely and irreversevely!!!
    - file 1 file 2 : delete file 1 and file 2
    - -i file 1 file 2 : the user is prompted before each file isi deleted
    - -r dir1 dir2 : directories dir 1 and dir 2 are deleted along with all of their contents
- mkdir dir : make a new directory

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
- [tab] key : automatically completes the document name
- [up arrow] key : Rewrite the commands user used before
- clear : clears the shell screen
- (help / man) command : show information about the command 
- exit : shut down the git terminal
- [\\] : ignore line change in command ("enter"), to enter a long command in multiple lines.

### Git commit

- git init : initializing a repository in an existing directory
- git status : checking repository status
- git add : adding a new file to be staged(tracked)
- git rm --cached file : unstaging a file
    - .gitignore : create gitignore files and manage deleted files separately
- git restore --staged <file> : unstaging a staged file
- git restore <file> : return to the file you recently committed
- git log : check all commit history
- git commit ( -m "commit message" ) : commmit
- git branch : checked the current branch
    - -m from to : change branch name

---
## 🗎Details
- Path notation
  >/ ➜ root 
  >. ➜  corrent directory
  >. . ➜ upper-level directory
  >~ ➜ home of current user
  >/[directory] ➜ absolute path
  > ./[directory] ➜  relative path
- Long format
![](https://miro.medium.com/max/1400/0*rLVhxj6mUY_GEH9c.png)
- Woildcards
    - *: All filenames
    - character* : All filenames that with the character
    - character*.extension : All filenames that begin with the character  and end with the characters '.extension'
    - word??? : Any filename that begins with the word followed by exactly 3 more characters
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

