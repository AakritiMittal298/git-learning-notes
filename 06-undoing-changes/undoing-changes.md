# Undoing changes safely

Before undoing work, inspect the current state:

```bash
git status
git diff
git diff --staged
```

## Unstage a file

```bash
git restore --staged <file>
```

This removes staged changes from the index while keeping the edits in the working tree.

Older equivalent syntax:

```bash
git reset HEAD <file>
```

## Discard unstaged edits

```bash
git restore <file>
```

This replaces the working-tree version with the index version. Uncommitted edits to that file are lost, so inspect or back up first.

## Restore a file from a particular commit

```bash
git restore --source=<commit-id> -- <file>
```

This updates the working-tree file from the chosen commit. Review and commit the result if you want to preserve it in current history.

## Important caution

Commands such as `git reset --hard` and `git clean -fd` can permanently discard local work. Understand their effect and back up important changes before using them.
