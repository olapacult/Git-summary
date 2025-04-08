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



## Working with Branches in Git

Branches allow you to work on different sections of a project without 
affecting the main branch. When the work is finished, a branch can be 
merged into the main project. You can also switch between branches 
and work on different tasks without them interfering with each other.

### Common Branch Commands

- **Create a new branch:**
`git branch <branch-name>'`

-**switch to another branch:**
`git checkout <branch-name>`

-**Create and switch to a new branch:**
`git checkout -b <branch-name>`

-**List all local branches:**
`git branch`

-**Delete a local branch:**
`git branch -d <branch-name>`

### Merging Branches
Merging a branch in Git involves combining the changes from one branch 
into another, typically to integrate new features or updates into the main codebase.

To merge changes from the selected branch into the current branch:
`git merge <branch-name>`

### Merging Branches
A conflict in Git occurs when changes made in two different branches are incompatible, 
meaning they affect the same part of the code in conflicting ways. This usually 
happens during a merge operation. Git is unable to automatically merge the changes 
and will mark the files with conflicts, requiring the user to manually resolve them 
by choosing which changes to keep or how to combine them.
