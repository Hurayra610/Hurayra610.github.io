# Git Command Guide

This README provides a list of essential Git commands along with descriptions of what they do. Git is a powerful version control system that helps developers collaborate, track changes, and manage project history efficiently.

## Table of Contents

- [Setup](#setup)
- [Basic Git Workflow](#basic-git-workflow)
- [Branching and Merging](#branching-and-merging)
- [Stashing](#stashing)
- [Remote Repositories](#remote-repositories)
- [Tagging](#tagging)
- [Advanced Commands](#advanced-commands)
- [Troubleshooting](#troubleshooting)
- [Resources](#resources)

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
