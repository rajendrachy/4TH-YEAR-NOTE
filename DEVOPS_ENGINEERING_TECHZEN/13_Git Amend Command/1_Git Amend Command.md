# Git Amend Command

## Introduction

The `git commit --amend` command is used to **modify the most recent commit**. It helps you fix mistakes like incorrect commit messages or missing changes without creating a new commit.

🎥 **Watch the Video:**  
https://youtu.be/3bpagBFwkOg?si=y2u8ugYi0Z6rXIEf

---

## What is Git Amend?

Git amend allows you to:
- Change the last commit message
- Add new changes to the last commit
- Replace the previous commit with a new one

---

## Change Last Commit Message

```bash
git commit --amend -m "New commit message"
```

Example:
```bash
git commit --amend -m "Fix login bug"
```

---

## Add Missing Changes to Last Commit

### Step 1: Add changes
```bash
git add .
```

### Step 2: Amend commit
```bash
git commit --amend
```

This opens the editor or updates the last commit with new changes.

---

## Important Notes

- Only works for the **most recent commit**
- It creates a **new commit replacing the previous one**
- Avoid using it after pushing to remote (can cause conflicts)

---

## When to Use Git Amend

- Forgot to add files in the last commit
- Need to fix commit message
- Small fixes before pushing code
- Cleaning up commit history

---

## Key Points

- `git commit --amend` edits the last commit
- Can change message or content
- Should be used before pushing to GitHub
- Helps maintain clean commit history