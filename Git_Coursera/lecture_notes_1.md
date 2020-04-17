### Directed Acyclic Graph (DAG)

Git models the relationships of commits with a DAG; the arrows point at a commit's parent(s).  A branch occurs if a commit has more than one child.  A merge occurs when a commit has more than one parent.  

### Git Objects

- Commit: a small text file
- Annotated tags: a permanent reference to a commit
- Tree: directories and filenames in the project
- Blob: the content of a file in the project

### Git IDs

40-character hexadecimal string; also known as object ID, SHA-1, hash and checksum.  Git IDs are SHA-1 values, and they are unique for a given piece of content (statistically speaking).

### Git References

User-friendly name that points to:
- a commit SHA-1 hash
- another reference, known as a symbolic reference

### Branch labels and HEAD

`master` is the default name of the main branch in the repository; branch label points to the most recent commit in the branch (the "tip of the branch").  HEAD is a reference to the current commit and usually points to the branch label of the current branch

### Appending tilde(~) to Git IDs and references

Refers to a prior commit
- `~` or `~1` = parent
- `~2` or `~~` = parent's parent

### Tags

Reference/label attached to a specific commit

- Lightweight: a simple reference to a commit
- Annotated: a full Git object that references a commit; includes tag author information, tag date, tag message, the commit ID

To tag a commit with a lightweight tag:
- `git tag <tagname> [<commit>]`
- `<commit> defaults to HEAD`

`git push` does not automatically transfer tags to the remote repository; to transfer a single tag: `git push <remote> <tagname>`; to transfer all of your tags: `git push <remote> --tags`

### Merging 

Main types of merges:
- Fast-forward merge
- merge commit
- squash merge
- rebase

Fast-forward merge moves the base branch label to the tip of the topic branch; it is possible if no other commits have been made to the base branch since branching. The following is how you perform a fast forward merge: `git checkout master` (switched to branch `master`), and then `git merger feature`.     







