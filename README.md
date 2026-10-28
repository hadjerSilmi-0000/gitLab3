# Git Lab 3: Branching, Merging & GitHub Flow

DevOps & Cloud Computing, Lab No. 03, Part A (Computer Science Department, 5th-year Software Engineering).

This repository documents a hands-on lab on Git branching, merging, conflict resolution, and the GitHub pull request workflow.

## What the lab covers

1. **Local repository:** three commits (`Version 1` to `Version 3`) on `main`
2. **Feature branch:** `feature1` with its own commits, isolated from `main`
3. **Bug fix on `main`:** a commit made while the feature was still in progress
4. **Merge:** `feature1` merged into `main` (merge commit, no conflict)
5. **Merge conflict:** `conflict` and `main` both edit the first line of `hello.txt`
6. **Conflict resolution:** markers removed, final content chosen, merge committed
7. **GitHub Flow:** owner and contributor roles, feature branch, pull request, review, merge, cleanup

## Repository contents

| File | Purpose |
|---|---|
| `hello.txt` | Edited across commits, used for the merge conflict |
| `feature.txt` | Created on `feature1`, merged into `main` |
| `bugfix.txt` | Created on `main` while the feature was in progress |
| `login.txt` | Added by the contributor through a pull request |

## GitHub Flow used in Part 7

```
main (stable)
  └── add-login-feature  → push → Pull Request → review → merge → delete branch
```

| Role | GitHub user | Responsibilities |
|---|---|---|
| Project owner | `hadjerSilmi-0000` | Publishes the repo, reviews and merges pull requests |
| Contributor | `Roumaissa-Kenn-H` | Branches, commits, pushes, opens the PR, applies review feedback |

## Useful commands

```bash
git log --oneline --graph --all   # view history and branches
git branch                        # list local branches
git merge <branch>                # merge a branch into the current one
git pull origin main              # sync with GitHub
```
