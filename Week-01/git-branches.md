# Git Branches

## Overview

Branches allow developers to work independently without affecting the stable version of a project. They are commonly used for developing new features, fixing bugs, updating documentation, or experimenting with new ideas.

---

## Why Branches Exist

Instead of modifying the `main` branch directly, developers create feature branches to isolate their work.

This allows multiple developers to work simultaneously without interfering with each other's changes.

---

## Typical Workflow

```text
main
    │
Create Branch
    │
Develop Feature
    │
Commit Changes
    │
Push Branch
    │
Open Pull Request
    │
Merge
    │
Delete Branch
```

---

## Local vs Remote Branches

### Local Branch

Exists only on your computer.

```bash
git branch
```

---

### Remote Branch

Exists on GitHub.

Created during the first push:

```bash
git push -u origin feature/my-branch
```

---

## Commands

| Command | Purpose |
|----------|---------|
| `git branch` | List local branches |
| `git switch branch-name` | Switch branches |
| `git switch -c branch-name` | Create and switch to a new branch |
| `git merge branch-name` | Merge another branch into the current branch |
| `git branch -d branch-name` | Delete a local branch |

---

## Pull Requests

A Pull Request (PR) is a request to merge changes from one branch into another.

The Pull Request process allows:

- Code review
- Team discussion
- Automated testing
- Approval before merging

---

## Key Takeaways

- Branches isolate work.
- `git push` uploads a branch but does not merge it.
- Pull Requests are reviewed before merging.
- Finished branches should be deleted after merging.