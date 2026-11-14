# Mission 6 — Git and GitHub

## 1. Task / objective

Understand version control and practise the Git workflow. Learn how to check repository status, stage changes, create commits, inspect commit history, create branches and collaborate through Pull Requests.

## 2. Work completed

### Task 6.1 — Basic Git workflow

I inspected my assignment repository using Git commands.

| Git operation | Command | What it does |
|---|---|---|
| Check repository status | `git status` | Shows modified, staged and untracked files and the current branch status. |
| Stage selected changes | `git add filename` | Selects specific changes to be included in the next commit. |
| Create a commit | `git commit -m "message"` | Saves the staged changes as a snapshot in the local Git history. |
| View commit history | `git log --oneline` | Displays previous commits in a compact format. |

### Difference between staging and committing

Staging means selecting the changes that should be included in the next commit. Committing records those staged changes in the local Git repository, creating a point in the project's history.

## Task 6.4 — Git Command Glossary

| Git Command | Explanation |
|---|---|
| `git init` | Initializes a new Git repository in the current directory. |
| `git status` | Displays the current branch and shows modified, staged and untracked files. |
| `git add <filename>` | Stages a selected file so its changes can be included in the next commit. |
| `git commit -m "message"` | Saves staged changes as a commit in the local Git history. |
| `git log --oneline` | Displays the commit history in a compact format. |
| `git branch` | Lists the available local branches. |
| `git branch <branch-name>` | Creates a new branch. |
| `git switch <branch-name>` | Switches to the specified branch. |
| `git push` | Publishes local commits to a remote repository. |
| `git pull` | Retrieves remote changes and integrates them into the current branch. |

### What is a Branch?

A branch is an independent line of development within a Git repository. It allows developers to work on changes without directly modifying the main branch.

### What is a Pull Request?

A Pull Request (PR) is a request to merge changes from one branch into another on GitHub. It allows other contributors to review, discuss and verify changes before they are merged.

### Why are Branches and Pull Requests Useful?

Branches allow multiple developers to work on different features independently. Pull Requests make collaboration easier by providing a place for code review, feedback and discussion before changes become part of the main project.