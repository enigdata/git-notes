## Saving changes

### git add

The `git add` command adds a change in the working directory to the staging area.  It tells Git that you want to include updates to a particular file in the next commit.  However, `git add` does not really affect the repo in any significant way, and changes won't happen until you `git commit`.

When you’re ready to save a copy of the current state of the project, you stage changes with `git add`.  After you are happy with the staged snapshot, you commit it to the project history with `git commit`.  The `git reset` is used to undo a commit or staged snapshot.  `git push` is then utilized to send the committed changes to remote repositories for other team members to view.

When used on its own, `git add` will promote pending changes from the working directory to the staging area.  The `git status` command is used to the examine the current state of the repo.  

### Git commit

Commits can be thought of as snapshots or milestones along the timeline of a Git project.  Just as the staging area if a buffer between the working directory and the project history, each developer's local repo is a buffer between their contributions and the central repo.  Git records the entire contents of each file in every commit.  Prior use of the `git add` command is required to select the changes that will be staged for the next commit.  

### Git diff

The `git diff` command is often used along with `git status` and `git log` to analyze the current state of a Git repo.  

### Git stash

`git stash` temporarily shelves changes you have made to your working copy so you can work on something else, and then come back and re-apply them later on.  Stashing is handy if you need to quickly switch context and work on something else, but you are mid-way through a code change and aren't quite ready to commit. The `git stash` command takes your uncommitted changes (both staged on unstaged), saves them away for later use, and then reverts them from your working copy.  You can reapply previously stashed changes with `git stash pop`; alternatively, you can reapply the changes to your working copy and keep them in your stash with `git stash apply`.  By default, Git won't stash changes made to untracked or ignored files.  So if we add a file but don't stage it (i.e. we don't run `git add`), `git stash` won't stash it.

Adding the `-u` option (or `--include-untracked`) tells `git stash` to also stash your untracked files.  You can also include changes to ignored files as well by passing the `-a` option (or `--all`) when running `git stash`.

To manage multiple 











