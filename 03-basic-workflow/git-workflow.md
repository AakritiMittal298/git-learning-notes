# Basic Git workflow

## Initialize a repository

```bash
mkdir git-practice
cd git-practice
git init
```

`git init` creates repository metadata in the current directory. It does not automatically stage files.

## Check repository status

```bash
git status
```

Status reports the current branch and whether files are untracked, modified, staged, or clean.

## Stage changes

```bash
git add README.md
git add .
```

The first stages one file. The second stages changes under the current directory. Review the staged result before committing.

## Commit staged changes

```bash
git commit -m "Add project README"
```

A commit records the staged snapshot with a message.

## Skip the explicit staging step

```bash
git commit -am "Update tracked files"
```

`-a` stages modifications and deletions of already tracked files. It does **not** include new untracked files.

## Commit message practices

Use concise, specific messages that explain the change, for example:

- `Add UART driver configuration`
- `Fix CAN receive timeout`
- `Update README with build instructions`

Keep unrelated changes in separate commits so each commit has a clear purpose.
