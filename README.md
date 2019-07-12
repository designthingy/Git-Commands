Git Commands
============

[Git Docs](https://git-scm.com/docs/)
[Writing good commit messages](https://github.com/erlang/otp/wiki/writing-good-commit-messages)

### Add Git credentials
| Command | Description |
| ------- | ----------- |
| `git config --global user.name [username]` | Add username |
| `git config --global user.email [email-address]` | Add email address |

### Remove Git credentials
| Command | Description |
| ------- | ----------- |
| `git config --global --unset credential.helper` | Unset Credential helper |
| -or- |
| `git config --system --unset credential.helper` | Unset Credential helper |

If non of the above will work then use below solution: [Windows](https://stackoverflow.com/a/39592537)

### Check Info
| Command | Description |
| ------- | ----------- |
| `git config --global --list` | Check username, email address and global options |
| `git config --global user.name` | Check username |
| `git config --global user.email` | check email address |

### Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Create a local copy/clone of a remote repository |

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
| `git push [remote name] [branch name]` | Push a branch to your remote repository |
| `git push -u [remote name] [branch name]` | Push changes to remote repository (and remember the branch) [see more](https://stackoverflow.com/a/18032002) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push [remote name] --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull [remote name] [branch name]` | Pull changes from remote repository |
| `git remote add [remote name] ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote remove [remote name]` | Remove remote name of the repository |
| `git remote set-url [remote name] ssh://git@github.com/[username]/[repository-name].git` | Change repository's origin url |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git diff [source branch] [target branch]` | Preview changes before merging |

