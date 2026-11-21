# Installation and configuration

## Install Git

Download Git for your operating system: https://git-scm.com/downloads

Verify installation:

```bash
git --version
```

## Configure author identity

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

These values are recorded in commits. `--global` applies to your user account; repository-local configuration can override it inside a repository:

```bash
git config user.name "Project Name"
git config user.email "project@example.com"
```

## Inspect configuration

```bash
git config --list
git config user.name
git config user.email
```

## Get help

```bash
git help
git help config
git config -h
```
