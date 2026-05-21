### Commands in Git

#### Git Bash Commands
    
1. ```cd``` <br />
    Tells the current directory

1. ```cd <folder-name>``` <br /> 
    Changes the current directory to the _folder-name_

1. ```cd ..``` <br />
    Moves one directory down in the hierarchy

1. ```cd ../..``` <br />
    Moves two directory down in the hierarchy

1. ```cd /~``` <br /> 
    Moves to the initial directory where Git is installed

1. ```mkdir <folder-name>``` <br /> 
    Create folders in the directory

1. ```touch <file-name>``` <br /> 
    Create files in the directory

1. ```mv <old-name> <new-name>``` <br /> 
    Rename the folder or file in the directory

1. ```mv <file-name> <destination-folder-name>/``` <br />
    Moves file from one directory to another directory

1. ```ls``` <br /> 
    Lists all the files and folders from the directory

1. ```cp <file-name> <folder-name>``` <br /> 
    Copies the files into the folder

1. ```rm <file-name>``` <br /> 
    Deletes the file

1. ```rm -rf <folder-name>``` <br /> 
   -  Deletes the folder
   - -r: Recursive - Allows the folder deletion along with its subfolders and files. Deletes the sub-directories also. <br />
    - -f: Force - Deletes directory without prompting for confirmation.

1. ```clear``` <br /> 
    Clears the Git Bash screen

#### Git Commands

_NOTE:_ <br />
In the command ```git reset --hard```, <br />
- ```git``` is the command
- ```reset``` is the subcommand
- ```hard``` is the option which is written using single hyphen (-) or double hyphen (--) <br />
<br />

_Basic Commands:_

1. ```git --version``` <br /> 
    Tells the version of Git installed in the system

1. ```git init``` <br />
    - Initial current folder of the directory as an empty Git repository
    - _.git_ file is created which symbolized Git repo
    - The current directory becomes the default _master/main_ branch

1. ```git status``` <br />
    Shows the status of the current repository

1. ```code <repo-name>/``` <br />
    - Opens the repo in the default code editor
    - Used when we are present in the directory where the repo is present

1. ```code .``` <br />
    - Opens the repo in the default code editor
    - Used when we are in the repo

1. ```code ~/.gitconfig``` <br />
    Used to check the configuration set for Git i.e. editor, username and email

    > Default editor for Git is Vim editor.

1. ```git <topic> --help``` <br />
    Provides information about the topic in the browser

1. ```git add <file-name>``` <br />
    Adds the file to the staging area

1. ```git add -A``` <br />
    Adds all the changes to the staging area

1. ```git add -u``` <br />
    Adds modified and deleted files to the staging area
    
1. ```git add .``` <br />
    Add new and multiple modified files to the staginga area

1. ```git rm --cached <file-name>``` <br />
    Unstages the file from the staging area

1. ```git commit -m "M"``` <br />
    - Used to commit the changes
    - Message of the commit is written in the CLI only

1. ```git commit``` <br />
    - Used to commit the changes
    - Message of the commit is written in the default editor

1. ```git commit -am "M"``` <br />
    - Used to stage and commit the files simulataneously
    - Used only for modified and updated files and not for newly created one

1. ```git commit --amend --no-edit``` <br />
    Updates the last commit with the modifications

1. ```git config --global user.name <name>``` <br />
    ```git config --global user.email <email-id>``` <br />
    Used to set the username and email id to Git

1. ```git config --global user.name``` <br />
    ```git config --global user.email``` <br />
    Used to check the username and email id linked to Git

1. ```git config --global core.editor "code--wait"``` <br />
    Used to set VS Code as the default editor

_History Commands:_

1. ```git log``` <br />
    - Used to check the commit history
    - Commit is shown with 40 character key and detailed commit message

1. ```git log --oneline``` <br />
    - Used to check the commit history
    - Commit is briefly shown - 7 character key and first line of the commit message

1. ```git log --oneline --graph``` <br />
    Generates a graph of the log history

1. ```git show HEAD``` <br />
    Gives detailed description for the HEAD commit

1. ```git show <commit-id>``` <br />
    Gives detailed description for the commit-id

1. ```git show HEAD~n``` <br />
    - Gives detailed description for the nth preeceded commit
    - Example: ```git show HEAD~1``` shows one commit before HEAD

1. ```git checkout <file-name>``` <br />
    - Unmodifies the changes in the file
    - Used after the files are modified and before they are staged
    - The changes in the files get reverted

1. ```git checkout .``` <br />
    Discard or unmodify the changes of all the files

1. ```git checkout <commit-id>``` <br />
    - Status of the project at that commit-id along with the commit message is seen
    - The remaining project status is not modified but we have just moved back in time 
    - HEAD is in the detatched state i.e. HEAD refers to the commit-id and the not to the master branch HEAD
    - Any modifications made during the detatched HEAD does not get saved
    - The change no longer exists since ```git checkout``` is only a read-only command
    - It is a safe command and if we want to do changes in different part of the code, we do so by using branches
    - To save the modifications made during the detatched HEAD state, create a new branch and the changes will get automatically saved

_Commands for Undoing Changes:_

1. ```git revert <commit-id>``` <br />
    - Undo the specific commit only and not the other commit
    - Opens the code editor for writing the commit message

1. ```git reset``` <br />
    - Undo the changes and commmits but it can be dangerous as it can delete the file permanently
    - Has three flags:
        - ```git reset --soft <commit-id>```
            - Files remains in the staging area even after the commits are removed from the commit history
            - For unstaging the files use - ```git reset .```
        - ```git reset --mixed <commit-id>``` <br />
            ```git reset <commit-id>```
            - It is the default reset command
            - Files are unstaged and the commits are removed from the commit history
        - ```git reset --hard <commit-id>```
            - Commits are messages are discarded simultaneously
            - No files are in the staging or unstaging area

    > The commit-id upto which we need to revert the changes are listed in the command

_Remote Commands:_

1. ```git remote add origin <https-link-of-the-remote-repo>``` <br />
    Connects local repo to the remote repo

1. ```git remote remove origin``` <br />
    Removes local repo and remote repo connection

1. ```git push origin main``` <br />
    Saves the modifications from local repo to remote repo

1. ```git push -u origin main``` <br />
    Sets the tracking branch and also saves the modifications from local repo to remote repo simulataneously

1. ```git pull origin main``` <br />
    Saves the modifications from remote repo to local repo
    > git pull = git fetch + git merge

1. ```git branch --set-upstream-to=origin/<branch>main```
    - Make the local branch main to track the remote branch from the origin
    - Git will push to and pull from the set branch

_Branching & Merging Commands:_

1. ```git branch <branch-name>``` <br />
    Creates the new branch

1. ```git branch``` <br />
    ```git branch --list``` <br />
    Lists the branches created in the repo with the current branch appearing with a '*' mark

1. ```git branch -D <branch-name>``` <br />
    Deletes the branch
    > The branch in which we are currently present doesn't gets deleted

1. ```git checkout <branch-name>``` <br />
    Used for switching between branches

1. ```git checkout -b <branch-name>``` <br />
    Creates and switches the branches at the same time

1. ```git push origin <branch-name>``` <br />
    - Pushes new branch from local repo to the remote repo
    - On GitHub, by compare and pull request the changes can be committed

1. ```git pull origin <branch-name>``` <br />
    - Pulls new branch from remote repo to the local repo
    - The branch will be pulled in the local repo but not shown. To see the branch, we need to track that branch using ```git checkout --track origin/<branch-name>```, which will list all the branches in the repo

1. ```git merge <branch-name>``` <br />
    Merges or joins the branch

1. ```git merge --abort``` <br />
    The merge conflicts are aborted but the changes remain as it is

_Advanced Commands:_

1. ```git diff``` <br />
    Provides difference between the current working directory and the staging area

1. ```git diff --staged``` <br />
    ```git diff --cached``` <br />
    Provides difference between the staging area and the last committed version

1. ```git diff <commit-id1> <commit-id2>``` <br />
    Provides the difference between commits

1. ```git diff HEAD~1``` <br />
    Provides the difference between current commit and previous commit

1. ```git diff <branch1> <branch2>``` <br />
    Provides the difference between tips of the two branches

1. ```git diff <commit-id>``` <br />
    Provides difference between the current working directory and the commit-id

1. ```git diff <branch>``` <br />
    Provides difference between current working directory and the branch

1. ```git config --global color.diff.old yellow``` <br />
    ```git config --global color.diff new blue``` <br />
    Use to change the default color in differences. Default colors are green (addition) and red (deletion)

1. ```git stash``` <br />
    Sometimes we need to quickly switch tasks or fix a bug, but we're not ready for committing the work, so the command lets us save the uncommitted changes and returns us to a clean working directory

---