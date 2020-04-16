## Saving changes

### git add

The `git add` command adds a change in the working directory to the staging area.  It tells Git that you want to include updates to a particular file in the next commit.  However, `git add` does not really affect the repo in any significant way, and changes won't happen until you `git commit`.

When you’re ready to save a copy of the current state of the project, you stage changes with `git add`.  After you are happy with the staged snapshot, you commit it to the project history with `git commit`.  The `git reset` is used to undo a commit or staged snapshot.  `git push` is then utilized to send the committed changes to remote repositories for other team members to view.

When used on its own, `git add` will promote pending changes from the working directory to the staging area.  The `git status` command is used to the examine the current state of the repo.  

### Git commit

Commits can be thought of as snapshots or milestones along the timeline of a Git project.  Just as the staging area if a buffer between the working directory and the project history, each developer's local repo is a buffer between their contributions and the central repo.  Git records the entire contents of each file in every commit.





