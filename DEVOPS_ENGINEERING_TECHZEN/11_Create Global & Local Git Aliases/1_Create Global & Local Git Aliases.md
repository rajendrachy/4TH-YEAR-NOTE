# Git Aliases (Global & Local)

## Introduction

Git aliases are shortcuts for long Git commands. They help you work faster by reducing typing and improving productivity.

🎥 **Watch the Video:**  
https://youtu.be/Jh6d83dAisE?si=G-R0k2HaWuvyyxXW

---

## What are Git Aliases?

Git aliases allow you to create **short commands** for frequently used Git operations.

Example:
```bash
git st   → git status
git co   → git checkout
git cm   → git commit
```

---

## Global Git Aliases

Global aliases work in **all repositories** on your system.

### Set a Global Alias

```bash
git config --global alias.st status
```

Now you can use:
```bash
git st
```

---

### More Examples

```bash
git config --global alias.co checkout
git config --global alias.cm commit
git config --global alias.br branch
```

---

## Local Git Aliases

Local aliases work **only inside a specific repository**.

### Set a Local Alias

```bash
git config alias.st status
```

This alias will only work in the current project.

---

## Advanced Alias Example

```bash
git config --global alias.lg "log --oneline --graph --all"
```

Usage:
```bash
git lg
```

Shows a clean visual commit history.

---

## When to Use Git Aliases

- To save time on repetitive commands
- To reduce typing errors
- To improve workflow efficiency
- To simplify complex Git commands

---

## Key Points

- Aliases are just shortcuts for Git commands
- Global aliases work everywhere
- Local aliases work only in one repo
- You can alias even complex commands
- Stored in Git configuration files