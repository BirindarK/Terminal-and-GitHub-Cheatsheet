# Terminal Command Cheatsheet 🖥️

## Keyboard Shortcuts in Terminal

*Command K* clears the commands in the terminal.

*Command S* saves the commands in the terminal.

*Control L* clears the commands in terminal, however, it allows you to scroll back to previous commands.

*Tab* auto completes commands.

*..* goes up to a previous directory (go up a level).

*.* goes to the current directory.

## General Commands used in Terminal

### List Command 

`ls` lists files within the current directory that user is in.

`ls -l` lists detailed information about the file, this includes the file permissions, number of links, owner, group, file size, modification time, file name.

`ls -a` lists all files within a directory, including any hidden file.

`ls -al` lists  all files and directories, including hidden ones, in the current directory.

### Changing Directory Command

`cd ` returns the user to the default/main directory.

`cd doc` typing this command and then using the tab key autocompletes the command to change the directory to the documents folder.

`cd ..` goes to the previous directory (go up a level) within the terminal 

### Print Working Directory Command

`pwd` prints the absolute path of the current working directory. Essentially, tells the user their location within the terminal.

### Make Directory Command

`mkdir` creates a new directory(folder) in the user's terminal location. 

### Make File Command

`touch` creates a new file in the user's terminal location. 

### Move Command 

`mv` renames a file or to change the location of the file within the terminal.

`mv` along with the old name of the file and the new name of the file, changes the file name and even the file type.

I.e. `mv [old_file_name.ext] [new_file_name.ext]` 

`mv` along with the file name and the new location, changes the actual location of the file within the terminal

I.e. `mv [file_name] [new_location]`

You can even combine the commands to move and rename the file at the same time 

I.e `mv [oldfile_name.ext] [new_location]/ [newfile_name.ext] `

NB: the name of the file is case sensitive, so it is very important to specify the extension of the file when naming it.

### Open Command

`open` opens any file or folder listed in terminal in the Mac Finder or any external program

`open [file_name]` opens the file in finder

`code .` opens the file within a text editor. In this case within VS Code.

### Copy Command

`cp` copies a file to another directory.

`cp -r` copies an entire directory (folder) to another directory.

### Delete Command 

`rm` permanently deletes a file from the device through running the terminal.

`rm -r` permanetly deletes an entire directory from the device through running the terminal. 

`rm -rf` deletes an entire directory with force (without any permissions)

## Terminal Commands for the use of Git

`git init` initialises the Git Repository

`git status`/ `gst` gives the status of the Git Repo

`git add [file_name]` tracks the changes of a specific file

`git add ` tracks all files

`git add --all` tracks the Git Repo

`git commit -m "first commit"` first commit (Title, Problem, Solution) saves all the work on git at the current stage.

Potential Errors:  

If you forget the end quotation and get the dquote message, simply add the end quote to solve.

If you forget to write a message and get an error, simply use *:wq* to solve. 

`git log` / `git show` lists the commit logs from most recent to previous. Essentially, shows who changed what code and when. To exit simply use *q*

`git restore` removes any unwanted changes from the code

`git config --global core.editor "code --wait` configures the git terminal to use visual code as a text editor.

`git revert [id_of_text_from_gitlog]` reverts the code to its original state from the saved checkpoints.

`git remote add origin` sets up a connection between the local Git repository and the remote repository

`git branch -M main` makes the current branch into the main branch.

`git push -u origin main` pushes the information from the local machine to the remote machine. That is, pushing information to GitHub.

`git pull origin main` pulls the information from the remote machine to the local machine. That is, pulling information from GitHub.

`git clone` clones a git repo.

El Fin... 

Extension

What are .gitignore files?

These are files that are used to ensure that files that are not tracked by Git remain untracked. This is useful when the user wants to ignore files and different file patterns before creating an new repository. It is particularly useful when engaged in large projects

Now we're Finished🎊
