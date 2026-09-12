# Git Clone Command

## Introduction

The `git clone` command is used to create a **local copy of a remote Git repository** (usually from GitHub). It downloads all files, history, and branches from the remote repository to your system.

🎥 **Watch the Video:**  
https://youtu.be/jrar75KBHbE?si=dXQWQhCy-Vu4sF_9

---

## What is Git Clone?

`git clone` helps you:
- Copy a repository from GitHub to your local machine
- Get full project history and files
- Start working on existing projects

---

## Basic Syntax

```bash
git clone <repository-url>
```

Example:

```bash
git clone https://github.com/user/repo.git
```

---

## Clone a Specific Branch

```bash
git clone -b <branch-name> <repo-url>
```

Example:

```bash
git clone -b dev https://github.com/user/repo.git
```

---

## What Happens After Cloning?

- A new folder is created
- All project files are downloaded
- Git history is included
- Remote origin is automatically set

Check remote:

```bash
git remote -v
```

---

## Difference: Git Clone vs Download ZIP

| Git Clone | ZIP Download |
|------------|--------------|
| Includes Git history | No history |
| Supports Git commands | Static files only |
| Can pull updates | Cannot update |
| Best for developers | Best for viewing only |

---

## When to Use Git Clone

- Starting work on a new project
- Contributing to open-source projects
- Downloading existing codebases
- Setting up development environments

---

## Key Points

- `git clone` copies a full repository
- It connects local repo to remote origin
- Supports branches and history
- Essential for real-world development workflows