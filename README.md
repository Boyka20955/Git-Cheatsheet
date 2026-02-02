# Git-Cheatsheet
Done By:Francis Irungu(firungu114@gmail.com)

🔹 1. Configuration & Setup

git config --global user.name "Name"
Sets your username for all repositories.

git config --global user.email "email"
Sets your email globally.

git config --list
Displays all Git configuration settings.

git config --global core.editor code
Sets VS Code as the default editor.

git help
Shows general Git help.

git help <command>
Shows help for a specific command.

🔹 2. Repository Creation

git init
Creates a new empty Git repository.

git clone <url>
Copies a remote repository to your machine.

git clone <url> <folder>
Clones repo into a specific folder.

🔹 3. Repository Status & Info

git status
Shows current repo status.

git status -s
Short status format.

git show
Shows details of the latest commit.

git show <commit>
Shows details of a specific commit.

🔹 4. Staging & File Tracking

git add <file>
Stages a file.

git add .
Stages all changes.

git add -A
Stages all changes (including deletions).

git reset <file>
Unstages a file.

git restore <file>
Discards file changes.

git restore --staged <file>
Removes file from staging area.

git rm <file>
Deletes a file and stages deletion.

git rm --cached <file>
Stops tracking file but keeps it.

git mv old new
Renames or moves a file.

🔹 5. Committing

git commit -m "message"
Commits staged changes.

git commit -am "message"
Adds and commits tracked files.

git commit --amend
Edits last commit.

git commit --amend -m "new message"
Changes last commit message.

🔹 6. Commit History & Logs

git log
Shows commit history.

git log --oneline
Compact commit history.

git log --graph
Visual commit tree.

git log --all --decorate --oneline --graph
Full visual history.

git reflog
Tracks all Git actions (recovery tool).

🔹 7. Branching

git branch
Lists branches.

git branch <name>
Creates new branch.

git branch -d <branch>
Deletes branch safely.

git branch -D <branch>
Forces branch deletion.

git branch -m <new-name>
Renames current branch.

🔹 8. Switching Branches

git checkout <branch>
Switches branch (old way).

git checkout -b <branch>
Creates and switches branch.

git switch <branch>
Modern way to switch branches.

git switch -c <branch>
Creates and switches branch.

🔹 9. Merging & Rebasing

git merge <branch>
Merges branch into current branch.

git merge --no-ff <branch>
Creates merge commit.

git merge --abort
Cancels merge.

git rebase <branch>
Re-applies commits on top of another branch.

git rebase --abort
Cancels rebase.

git rebase --continue
Continues rebase after conflict resolution.

git cherry-pick <commit>
Applies specific commit.

🔹 10. Remote Repositories

git remote
Lists remote names.

git remote -v
Shows remote URLs.

git remote add origin <url>
Adds remote repository.

git remote remove origin
Removes remote.

git fetch
Downloads changes only.

git pull
Fetches and merges changes.

git pull --rebase
Pulls using rebase.

git push
Pushes commits to remote.

git push -u origin <branch>
Sets upstream branch.

git push --force
Force push (dangerous).

🔹 11. Undo & Reset

git reset --soft HEAD~1
Undo commit, keep changes staged.

git reset --mixed HEAD~1
Undo commit, keep changes unstaged.

git reset --hard HEAD~1
Deletes commit and changes.

git checkout -- <file>
Discards file changes.

git revert <commit>
Creates commit that undoes changes.

🔹 12. Diff & Inspection

git diff
Shows unstaged changes.

git diff --staged
Shows staged changes.

git diff branch1 branch2
Compares branches.

git blame <file>
Shows who changed each line.

🔹 13. Stashing

git stash
Saves uncommitted work.

git stash list
Shows stash entries.

git stash pop
Restores last stash.

git stash apply
Applies stash without deleting it.

git stash drop
Deletes stash.

git stash clear
Deletes all stashes.

🔹 14. Tags & Releases

git tag
Lists tags.

git tag v1.0
Creates lightweight tag.

git tag -a v1.0 -m "message"
Creates annotated tag.

git push origin --tags
Pushes tags to remote.

🔹 15. Cleanup & Maintenance

git clean -f
Removes untracked files.

git clean -fd
Removes untracked files and folders.

git gc
Optimizes repository.

git fsck
Checks repo integrity.

🔹 16. Archives & Export

git archive --format=zip HEAD > project.zip
Exports repo as ZIP.

🔹 17. Submodules

git submodule add <repo>
Adds submodule.

git submodule update
Updates submodule.

git submodule init
Initializes submodules.

🔹 18. Advanced Recovery

git reflog
Shows all HEAD movements.

git reset --hard <reflog-id>
Restores lost commits.
