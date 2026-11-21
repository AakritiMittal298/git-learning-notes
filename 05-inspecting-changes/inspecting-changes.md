# Inspecting changes

## Short status

```bash
git status --short
```

Common markers:

- `??` – untracked file.
- ` M` – unstaged working-tree modification.
- `M ` – staged modification.
- `A ` – staged addition.
- `D ` – staged deletion.

The first column describes the index; the second describes the working tree.

## View unstaged differences

```bash
git diff
```

Shows changes in the working directory that are not staged.

## View staged differences

```bash
git diff --staged
```

Shows what is currently staged for the next commit. `git diff --cached` is an equivalent form.

## View commit history

```bash
git log
git log --oneline
git log --oneline --graph --decorate --all
```

## Inspect a commit

```bash
git show <commit-id>
```

This displays commit metadata and its patch. A shortened commit ID works when it is unambiguous.

## Visual diff tools

A configured visual diff tool can help review larger changes:

```bash
git difftool
```
