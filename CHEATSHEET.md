# Git command cheat sheet

| Task | Command |
|---|---|
| Check version | `git --version` |
| Set global name | `git config --global user.name "Name"` |
| Set global email | `git config --global user.email "email"` |
| Initialize repository | `git init` |
| Check status | `git status` |
| Short status | `git status --short` |
| Stage one file | `git add file` |
| Stage changes under current directory | `git add .` |
| Commit staged changes | `git commit -m "Message"` |
| Commit tracked modifications/deletions | `git commit -am "Message"` |
| Remove tracked file | `git rm file` |
| Rename tracked file | `git mv old new` |
| Unstaged diff | `git diff` |
| Staged diff | `git diff --staged` |
| View history | `git log --oneline` |
| Inspect commit | `git show <commit>` |
| Unstage file | `git restore --staged file` |
| Discard unstaged edits | `git restore file` |
| Restore file from commit | `git restore --source=<commit> -- file` |

## Remember

- `git add` stages changes; it does not create a commit.
- `git commit` records the staged snapshot.
- `git diff` and `git diff --staged` inspect different areas.
- `git commit -am` excludes untracked files.
- Review `git status` before and after operations that alter the index or working tree.
