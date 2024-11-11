# Git Command Guide

This Document provides a list of essential Git commands along with descriptions of what they do. Git is a powerful version control system that helps developers collaborate, track changes, and manage project history efficiently.

## Table of Contents

- [Setup](#setup)
- [Basic Git Workflow](#basic-git-workflow)
- [Branching and Merging](#branching-and-merging)
- [Stashing](#stashing)
- [Remote Repositories](#remote-repositories)
- [Tagging](#tagging)
- [Advanced Commands](#advanced-commands)
- [Troubleshooting](#troubleshooting)

---

## Setup

### 1. **`git init`**

- Initialize a new Git repository in the current directory.

```bash
git init
```

### 2. **`git config`**

- Set user configuration options like username and email.

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### 3. **`git clone`**

- Clone a remote repository to your local machine.

```bash
git clone <repository_url>
```

## Basic Git Workflow

### 4. **`git status`**

- Check the status of your working directory and staging area.

```bash
git status
```

### 5. **`git add`**

- Add changes from the working directory to the staging area.

```bash
git add <file>
git add .  # Add all changes
```

### 6. **`git commit`**

- Commit staged changes to the repository with a message.

```bash
git commit -m "Commit message"
```

### 7. **`git log`**

- Show commit history.

```bash
git log
```

### 8. **`git diff`**

- Show changes between commits, working directory, and staging area.

```bash
git diff
```

## Branching and Merging

### 9. **`git branch`**

- List, create, or delete branches.

```bash
git branch                 # List all branches
git branch <branch_name>   # Create a new branch
git branch -d <branch_name> # Delete a branch
```

### 10. **`git checkout`**

- Switch to another branch or commit.

```bash
git checkout <branch_name>
git checkout -b <new_branch_name>  # Create and switch to a new branch
```

### 11. **`git merge`**

- Merge the specified branch into the current branch.

```bash
git merge <branch_name>
```

## Stashing

### 12. **`git stash`**

- Temporarily save changes without committing them.

```bash
git stash
git stash pop    # Apply the latest stash
git stash list   # List all stashes
```

## Remote Repositories

### 13. **`git remote`**

- Manage remote repository connections.

```bash
git remote add <name> <url>    # Add a new remote
git remote -v                  # List all remotes
git remote remove <name>       # Remove a remote
```

### 14. **`git push`**

- Push commits to a remote repository.

```bash
git push <remote> <branch>
git push -u origin <branch>    # Set up tracking and push
```

### 15. **`git pull`**

- Fetch and merge changes from a remote repository.

```bash
git pull <remote> <branch>
```

### 16. **`git fetch`**

- Download commits and files from a remote repository without merging.

```bash
git fetch <remote>
```

## Tagging

### 17. **`git tag`**

- Create, list, or delete tags.

```bash
git tag                   # List tags
git tag <tag_name>        # Create a new tag
git tag -d <tag_name>     # Delete a tag
git push origin <tag_name> # Push a tag to a remote
```

## Advanced Commands

### 18. **`git rebase`**

- Reapply commits on top of another base commit.

```bash
git rebase <branch>
```

### 19. **`git reset`**

- Unstage or discard changes.

```bash
git reset <file>          # Unstage file
git reset --hard          # Discard all changes in working directory
```

### 20. **`git revert`**

- Create a new commit that undoes changes from a previous commit.

```bash
git revert <commit_id>
```

## Troubleshooting

### 21. **`git clean`**

- Remove untracked files from the working directory.

```bash
git clean -f    # Remove untracked files
git clean -fd   # Remove untracked files and directories
```

### 22. **`git cherry-pick`**

- Apply specific commits from one branch into another.

```bash
git cherry-pick <commit_id>
```

### 23. **`git archive`**

- Create an archive of files from a repository.

```bash
git archive --format=zip HEAD > archive.zip
```

### 24. **`git blame`**

- Show what revision and author last modified each line of a file.

```bash
git blame <file>
```

### 25. **`git bisect`**

- Use binary search to find the commit that introduced a bug.

```bash
git bisect start
git bisect bad           # Mark the current commit as bad
git bisect good <commit> # Mark a known good commit
```
