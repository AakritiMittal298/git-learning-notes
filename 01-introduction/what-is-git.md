# Introduction to Git

## What is Git?

Git is a distributed version control system. It records changes to files over time so that work can be reviewed, compared, restored, and shared.

## Why use version control?

- Maintain a history of project changes.
- Work on features independently using branches.
- Collaborate without manually passing source folders around.
- Identify when and why a change was introduced.

## Repository

A Git repository contains project files and the metadata/history Git uses to track them. The `.git` directory stores repository metadata.

## Three important areas

1. **Working directory** – files currently being edited.
2. **Staging area (index)** – selected changes prepared for the next commit.
3. **Repository history** – committed snapshots.

Typical flow: edit → stage → commit.

## Snapshot concept

A commit records the staged state of the project, along with metadata such as author, timestamp, parent commit, and message. Git stores content efficiently and commits form a history graph.
