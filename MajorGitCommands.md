# all major git commands

git config –global user.name “[name]” -> sets the author name respectively to be used with your commits
git config –global user.email “[email address]” -> sets the email address respectively to be used with your commits

git clone [HTTP Code Path] -> Create a local copy of a remote repository

cd [Folder Path] -> Navigate to respective folder name

git status -> Lists all the files that have to be committed

git fetch --all -> Download all branches

git branch -> List branches (the asterisk denotes the current branch)
git branch -a -> List all branches (local and remote)
git branch [Branch Name] -> Creates a new branch
git branch -d [Branch Name] -> Deletes the feature branch

git checkout -b [Branch Name] - Creates a new branch and also switches to it
git checkout [Branch Name] -> To switch from one branch to another

git init [Repository Name] -> Start a new repository

git add [File Name] -> Add a file to the staging area
git add * -> Add one or more to the staging area

git commit -m “[ Type in the commit message]” -> records or snapshots the file permanently in the version history
git commit -a -> Commits any files you’ve added with the git add command and also commits any files you’ve changed since then.

git rm [file] -> Deletes the file from your working directory and stages the deletion
git rm -r [file-name.txt] -> Remove a file (or folder)

git restore --staged [filename] -> Restoring files in the working tree

git revert -> Making a new commit that reverts the changes made by other commits

git reset -> Updating your branch, moving the tip in order to add or remove commits from the branch

git log -> List the version history for the current branch
git log --summary -> View changes (detailed)
git log --oneline -> View changes (detailed)
git log –follow[file] -> Lists version history for a file, including the renaming of files also

git diff -> Shows the file differences which are not yet staged
git diff –staged -> Shows the differences between the files in the staging area and the latest version present
git diff [first branch] [second branch] -> Shows the differences between the two branches mentioned

git reset [file] -> Unstages the file, but it preserves the file contents
git reset [commit] -> Undoes all the commits after the specified commit and preserves the changes locally
git reset –hard [commit] -> Discards all history and goes back to the specified commit

git show [commit] -> Shows the metadata and content changes of the specified commit

git merge [Branch Name] -> Merges the specified branch’s history into the current branch
git merge [source branch] [target branch] -> Merge a branch into a target branch

git remote add [variable name] [Remote Server Link] -> connect your local repository to the remote server

git push -u origin [Branch Name] -> Push changes to remote repository (and remember the branch) | Mention -u at starting at once 
git push origin [Branch Name] -> Push a branch to your remote repository
git push -> Push changes to remote repository (Remembered Branch)
git push origin --delete [Branch Name] -> Delete a remote branch
git push [variable name] master -> Sends the committed changes of master branch to your remote repository
git push [variable name] [Branch Name] -> Sends the branch commits to your remote repository
git push –all [variable name] -> Pushes all branches to your remote repository
git push [variable name] :[branch name] -> Deletes a branch on your remote repository

git pull -> Update local repository to the newest commit
git pull origin [Branch Name] -> Pull changes from remote repository
git pull [Repository Link] -> Fetches and merges changes on the remote server to your working directory

git stash -> Stash changes in a dirty working directory
git stash save -> Restores the most recently stashed files
git stash list -> Lists all stashed changesets
git stash drop -> Discards the most recently stashed changeset
git stash clear -> Remove all stashed entries
