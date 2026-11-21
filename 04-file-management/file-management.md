# File management

## Remove a tracked file

```bash
git rm old-file.c
git status
git commit -m "Remove obsolete file"
```

`git rm` removes the file from the working tree and stages the deletion.

## Rename or move a tracked file

```bash
git mv old-name.c new-name.c
git status
git commit -m "Rename module source file"
```

Git stores snapshots; rename detection is inferred when comparing changes.

## Ignore generated or local files

Create `.gitignore` in the repository root. Example for a software project:

```gitignore
# Build output
build/
*.o
*.elf
*.map

# IDE / local settings
.vscode/
.idea/

# Logs
*.log
```

Adjust patterns to the project. `.gitignore` does not stop tracking files already committed. To remove a file from Git tracking while keeping the local copy:

```bash
git rm --cached path/to/file
```

Then commit the index change and updated `.gitignore`.
