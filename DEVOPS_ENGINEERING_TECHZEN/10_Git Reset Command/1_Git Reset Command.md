# Git Reset Command

## Introduction

The `git reset` command is used to move the current branch (HEAD) to a previous commit. It can also be used to unstage files or remove changes depending on the option used.

Unlike `git revert`, `git reset` can rewrite commit history, so it should be used carefully.

🎥 **Watch the Video:**  
https://youtu.be/qL57wSk9UVw?si=__eIHi1IrNeil5FJ

---

## What You Will Learn

- What Git Reset is and how it works
- Understanding `--soft`, `--mixed`, and `--hard` reset options
- Difference between Git Reset and Git Revert
- Practical use of `HEAD~1` to undo commits
- Real-world scenarios of using reset effectively


# Git Reset Command Notes

## Introduction

The `git reset` command is used to move the current branch (HEAD) to a previous commit. It helps in undoing commits, unstaging files, or removing changes depending on the option used.

It is a powerful command because it can **modify commit history**, so it should be used carefully.

🎥 **Watch the Video:**  
https://youtu.be/qL57wSk9UVw?si=__eIHi1IrNeil5FJ

---

## Types of Git Reset

### 1. Soft Reset

```bash
git reset --soft <commit>
```

- Moves HEAD to a previous commit
- Keeps changes staged (in index)
- Does not remove working directory changes

Use case: Undo commit but keep changes ready for recommit.

---

### 2. Mixed Reset (Default)

```bash
git reset --mixed <commit>
```

or

```bash
git reset <commit>
```

- Moves HEAD to previous commit
- Unstages files
- Keeps changes in working directory

Use case: Undo staging but keep code changes.

---

### 3. Hard Reset

```bash
git reset --hard <commit>
```

- Moves HEAD to previous commit
- Removes staged changes
- Deletes all working directory changes

Use case: Completely discard changes

Warning: Data is permanently lost if not committed.

---

## Common Example

```bash
git reset HEAD~1
```

- Moves branch back by 1 commit
- Default is mixed reset

---

## Git Reset vs Git Revert

| Git Reset | Git Revert |
|-----------|------------|
| Deletes/rewrites history | Keeps history |
| Local use recommended | Safe for shared repos |
| Can remove commits | Creates new commit |

---

## Key Points

- HEAD represents the current position in Git history
- `reset` moves HEAD to a different commit
- Use `soft`, `mixed`, or `hard` depending on need
- Avoid using reset on shared/public branches
- Prefer `revert` for already pushed commits
