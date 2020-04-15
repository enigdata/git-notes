## Git Basics

`git init`: Create empty Git repo in the specified directory

`git clone <repo>`: Clone repo located at `<repo>` onto local machine

`git add <directory>`: Stage all changes in `<directory>` for the next commit

`git commit -m "<message>"`: Add commit message for reference

`git status`: List which files are staged, unstaged, and untracked

`git log`: Display the entire commit history using the default format

`git diff`: Show unstaged changes

## Undoing Changes

`git revert <commit>`: Create new commit that undoes all of the changes made in `<commit>`

`git reset <file>`: Remove `<file>` from the staging area, but leave the working directory unchanged; this unstages a file without overwriting any changes

`git clean -n`: Shows which files would be removed from working directory

