Connect local repo to remote repo: `git remote add origin <url_to_github_repo>`

Show current branch: `git branch --show-current`

Retrieve changes from remote repository, but does not automatically merge them into local branch: `git fetch`
- `git merge` to do the second half

To undo a `git add .`: `git reset`

Undo all changes back to last commit (lose uncommitted changes): `git reset --hard HEAD`

Remove all untracked files: `git clean -f`

Branches: `git branch [-ad] <name>`

Don't have all branches? `git fetch --all

Show changelog: `git log --oneline --decorate --color --graph`