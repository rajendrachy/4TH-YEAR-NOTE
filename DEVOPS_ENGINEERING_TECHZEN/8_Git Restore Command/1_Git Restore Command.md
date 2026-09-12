# 🔄 Git Restore Command

Learn how to use the `git restore` command to undo changes in your working directory and safely recover files in Git.

🎥 **Watch the Video:**  
https://youtu.be/9NcXOSXIOOQ?si=hLDpEJhmQv_ozdv-

> 💡 **Recommended:** Learn `git restore` after understanding basic Git commands to manage and undo file changes safely.



# Git Restore Command

## What is `git restore`?

The `git restore` command is used to discard changes in your working directory and restore files to their previous state. It is commonly used to undo accidental modifications before committing changes.

---

## Common Commands

### Restore a Single File

```bash
git restore <file-name>
```

Example:

```bash
git restore index.html
```

Restores the file to its last committed state.

---

### Restore All Modified Files

```bash
git restore .
```

Restores all modified files in the current directory.

---

### Restore a File from the Latest Commit

```bash
git restore --source=HEAD <file-name>
```

Example:

```bash
git restore --source=HEAD app.js
```

Restores the specified file from the latest commit (`HEAD`).

---

### Unstage a File

```bash
git restore --staged <file-name>
```

Example:

```bash
git restore --staged app.js
```

Removes the file from the staging area while keeping the changes in your working directory.

---

## When to Use `git restore`

- Undo accidental changes in a file.
- Restore a file to its last committed version.
- Remove files from the staging area.
- Recover files before creating a commit.

---

## Key Points

- `git restore` only affects your local repository.
- It does not modify the commit history.
- It is safe to use before committing changes.
- Once local changes are restored, they cannot be recovered unless they were committed or backed up.