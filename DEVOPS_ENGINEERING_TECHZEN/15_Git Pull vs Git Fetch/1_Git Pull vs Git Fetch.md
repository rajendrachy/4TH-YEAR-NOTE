# Git Pull vs Git Fetch

## Introduction

Both `git pull` and `git fetch` are used to update your local repository with changes from a remote repository, but they work in different ways.

🎥 **Watch the Video:**  
https://youtu.be/xvU1zboOtj0?si=dsT7kWFjThk0LKGv

---

## What is Git Fetch?

`git fetch` downloads the latest changes from the remote repository but **does not merge them** into your current branch.

### Command:
```bash
git fetch origin
```

### What it does:
- Downloads new commits
- Updates remote tracking branches
- Does NOT change your working code

---

## What is Git Pull?

`git pull` is a combination of **fetch + merge**. It downloads changes and automatically merges them into your current branch.

### Command:
```bash
git pull origin main
```

### What it does:
- Downloads changes from remote
- Automatically merges into local branch
- Updates your working directory

---

## Difference Between Git Pull and Git Fetch

| Git Fetch | Git Pull |
|-----------|----------|
| Only downloads changes | Downloads + merges changes |
| Does not modify working code | Updates working code immediately |
| Safe to review changes first | Directly applies changes |
| Manual merge required | Auto merge |

---

## When to Use

### Use Git Fetch when:
- You want to review changes before applying
- Working on important or large projects
- Avoiding automatic merge conflicts

### Use Git Pull when:
- You want quick updates
- Working on small or personal projects
- You trust remote changes

---

## Key Points

- `git fetch` = download only
- `git pull` = download + merge
- Fetch is safer for reviewing changes
- Pull is faster but less controlled
- Both help keep your repository updated