## Git Basics

`git init`: Create empty Git repo in the specified directory

`git clone <repo>`: Clone repo located at `<repo>` onto local machine

`git remote add <name> <url>`: Greate a connection to a remote repo

`git fetch <remote> <branch>`: Fetches a specific `<branch>`, from the repo

`git pull <remote>`: Fetch the specified remote's copy of current branch and immediately merge it into the local copy

`git push <remote> <branch>`: Push the branch to `<remote>`, along with necessary commits and objects; creates named branch in the remote repo if it doesn't exist

`git add <directory>`: Stage all changes in `<directory>` for the next commit

`git commit -m "<message>"`: Add commit message for reference

`git status`: List which files are staged, unstaged, and untracked

`git log`: Display the entire commit history using the default format

`git diff`: Show unstaged changes

## Git Config

`git config --global user.name <name>`: Define the author name to be used for all commits by the current user

`git config --global user.email <email>`: Define the author email to be used for all commits by the current user

`git config --global alias. <alias-name> <git-command>`: Create shortcut for a Git command

`git config --global --edit`: Open the global configuration file in a text editor for manual editing

## Git Branches

`git branch`: List all of the branches in your repo; add a `<branch>` argument to create a new branch with the name `<branch>`

`git checkout -b <branch>`: Create and check out a new branch named `<branch>`; drop the `-b` flag to checkout an existing branch

`git merge <branch>`: Merge `<branch>` into the current branch

## Undoing Changes

`git revert <commit>`: Create new commit that undoes all of the changes made in `<commit>`

`git reset <file>`: Remove `<file>` from the staging area, but leave the working directory unchanged; this unstages a file without overwriting any changes

`git clean -n`: Shows which files would be removed from working directory

## Rewriting Git History

`git commit --amend`: Edit the last commit's message

`git rebase <base>`: Rebase the current branch onto `<base>`. `<base>` can be a commite ID, branch name, a tag, or a relative reference to HEAD

## Git Diff

`git diff HEAD`: Show difference between working directory and last commit

`git diff --cached`: Show difference between staged changes and last commit



