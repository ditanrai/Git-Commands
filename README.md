# Git-Commands

####TO PULL AND TO PUSH THE GIT REPOSITORY FROM SERVER AND LOCAL MECHINE.


1. Create folder and new repository in local machine and initilize it.

=> git init


2. Check current status.

=> git status


3. Check the branch in Master.

=> git branch


4. Create new branch.

=> git checkout -b {"branch-name": given by us} or {"topic1/storynumber1"}


5. Connect local repository to remote repository.

=> git remote add origin {"repository-path"}


6. Pull changes from remote repository {Pulling file from remote server}.

=> git pull origin {"remote-master-name"} or {"remote-branch-name"}


7. Commit(save) the changes you made.

=> git commit -m "comments"


8. Adding file to the staging area.

=> git add {"file-name": adding single file}

=> git add . {To add all file}


9. Again commit.

=> git commit -m "comments"


10. Push the branch to your remote repository.

=> git push

or

=> git push origin {"branch-name": given by us}

or

=> git push --set-upsteam origin {"branch-name": given by us}
 
 

==================================================================



####TO UPLOAD THE FILES AND PROJECT FROM LOCAL MECHINE TO REMOTE SERVER.

1. First create "New repository" in GitHub.


2. Go to the local project folder where all the project's files are resides and inside the project folder open the command prompt "cmd"


3. Before continue further we need to remove all the existing git files from the folder.

=> rd .git /S/Q


4. Initilize the git 

=> git init


5. Add files to the git 

=> git add . {adding all the files inside the folder}


6. Commit all the changes made by us

=> git commit -m "comments"


7. Connecting local repository to the remote repository

=> git remote add origin {"repository-path"}


8. Uploading the file or project into the git repository

=> git push -u origin master

or

=> git push --push-upstream origin {"branch-name" or "master"}




============================================================================





Git Commands
============


A list of my commonly used Git commands



### Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |

### Basic Snapshotting

| Command | Description |
| ------- | ----------- |
| `git status` | Check status |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git add -A` | Add all new and changed files to the staging area |
| `git commit -m "[commit message]"` | Commit changes |
| `git rm -r [file-name.txt]` | Remove a file (or folder) |

### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch name]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it |
| `git branch -m [old branch name] [new branch name]` | Rename a local branch |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |

### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git log --oneline` | View changes (briefly) |
| `git diff [source branch] [target branch]` | Preview changes before merging |
