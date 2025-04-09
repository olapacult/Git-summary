# Git Summary

**Author** Aleksandra Pacułt

**Date** 8.04.2025

**Description** This repository contains a summary of the most important 
Git commands and concepts.

---

## Git - what it is?

Git is a distributed version control system used to track changes 
in files, most commonly in the context of collaborative software development.
It was designed with key goals in mind: high performance, strong data integrity, 
and the ability to support distributed, non-linear workflows - allowing 
thousands of branches to be developed in parallel across multiple machines.


## Basic commands in Git

- **Starting a repository:**
```
git init                # Initialize a new Git repository
git clone <url>         # Clone an existing repository
```

- **Saving changes**
```
git status              # Show current status of the working directory
git add <file>          # Stage a file for commit
git add .               # Stage all changed files
git commit -m "Message" # Commit staged changes with a message
```

- **Working with Remotes**
```
git remote -v           # List remotes
git push                # Push commits to remote
git pull                # Pull latest changes from remote
git fetch               # Fetch changes without merging
```

## Working with Branches in Git

Branches in Git are used to develop different features or changes independently 
from the main codebase. They allow you to make changes, test ideas, or 
fix bugs without affecting the working version of your project.

### Common Branch Commands

- **Create a new branch:**
`git branch <branch-name>`

- **Switch to another branch:**
`git checkout <branch-name>`

- **Create and switch to a new branch:**
`git checkout -b <branch-name>`

- **List all local branches:**
`git branch`

- **Delete a local branch:**
`git branch -d <branch-name>`

### Merging Branches
Merging a branch in Git involves combining the changes from one branch 
into another, typically to integrate new features or updates into the main codebase.

To merge changes from the selected branch into the current branch:
`git merge <branch-name>`

### Merge conflict

A conflict in Git occurs when changes made in two different branches are incompatible, 
meaning they affect the same part of the code in conflicting ways. This usually 
happens during a merge operation. 

How to solve it?

1. Git will indicate which files have conflicts after a merge attempt.
2. Git marks the conflicting areas in the file with special markers 
(<<<<<<<, =======, >>>>>>>), showing both versions of the code.
3. Manually edit the file to decide which changes to keep or how to combine them.
4. Mark the conflict as resolved: After editing, save the file and run git add <filename> to mark the conflict as resolved.
5. Finally, commit the resolved changes with git commit to finish the merge process.
