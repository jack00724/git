cat << 'EOF' > README.md
# 🚀 Complete Git & GitHub Master Guide for DevOps Engineers

A comprehensive, production-ready reference guide covering basic, intermediate, and advanced Git workflows, commands, and GitHub collaboration strategies.

---

## 📌 Table of Contents
1. [Core Daily Workflow](#1-core-daily-workflow)
2. [Branching & Merging](#2-branching--merging)
3. [Undoing Changes & Rollbacks](#3-undoing-changes--rollbacks)
4. [Stashing & Cherry-Picking](#4-stashing--cherry-picking)
5. [Advanced History & Inspection](#5-advanced-history--inspection)
6. [Remote Repositories & GitHub](#6-remote-repositories--github)
7. [DevOps Workflows & GitHub Actions](#7-devops-workflows--github-actions)
8. [Quick Reference Command Matrix](#8-quick-reference-command-matrix)

---

## 1. Core Daily Workflow

| Command | Category | What It Does | Real-World Analogy |
| :--- | :--- | :--- | :--- |
| `git config --global user.name "..."` | **Setup** | Sets your username for all commits. | Writing your name on your notebook cover. |
| `git config --global user.email "..."` | **Setup** | Sets your email for all commits. | Adding contact details to your notebook. |
| `git init` | **Setup** | Turns current folder into a Git repo. | Buying a fresh journal and opening page 1. |
| `git status` | **Inspection** | Shows untracked/staged/modified files. | Looking at your desk to see what needs organizing. |
| `git add <file>` | **Staging** | Moves specific file changes to staging area. | Lining up one person for a group photo. |
| `git add .` | **Staging** | Stages ALL current changes in directory. | Lining up everyone for the group photo. |
| `git commit -m "message"` | **Saving** | Saves a permanent snapshot with message. | Clicking the shutter button to take the photo. |
| `git log` | **Inspection** | Shows full commit history details. | Opening a detailed logs notebook. |
| `git log --oneline` | **Inspection** | Displays concise, 1-line commit list. | Flipping quickly through your photo album. |

---

## 2. Branching & Merging

| Command | Category | What It Does | Real-World Analogy |
| :--- | :--- | :--- | :--- |
| `git branch` | **Branching** | Lists all local branches. | Checking parallel universes available. |
| `git branch <name>` | **Branching** | Creates a new branch from current code. | Drafting a copy of a draft document. |
| `git switch <name>` | **Branching** | Switches active working directory to branch. | Stepping into a parallel workspace. |
| `git switch -c <name>` | **Branching** | Creates AND switches to new branch at once. | Teleporting directly into a new sandbox. |
| `git merge <branch>` | **Merging** | Combines changes from branch into current. | Pouring experimental work into main project. |
| `git rebase main` | **Rebasing** | Re-applies commits on top of latest main. | Moving your edits to sit on top of newest base. |
| `git branch -d <name>` | **Cleanup** | Deletes a safely merged branch. | Shredding finished scrap paper. |

---

## 3. Undoing Changes & Rollbacks

| Command | Category | What It Does | Real-World Analogy |
| :--- | :--- | :--- | :--- |
| `git restore --staged <file>` | **Unstaging** | Removes file from staging area. | Asking someone to step out of photo lineup. |
| `git restore <file>` | **Discard** | Erases local changes in file back to snapshot. | Smudging out unstained pencil marks. |
| `git revert <commit-hash>` | **Rollback** | Safely undoes a commit by making a NEW commit. | Writing a correction post in a public ledger. |
| `git reset --soft HEAD~1` | **Reset** | Moves HEAD back 1 commit; keeps changes staged. | Unpacking a package but keeping items ready. |
| `git reset --mixed HEAD~1` | **Reset** | Moves HEAD back 1 commit; keeps changes unstaged. | Unpacking a package and putting items on desk. |
| `git reset --hard <hash>` | **Reset** | DANGEROUS: Wipes ALL local changes back to hash. | Shredding everything built since last check. |

---

## 4. Stashing & Cherry-Picking

| Command | Category | What It Does | Real-World Analogy |
| :--- | :--- | :--- | :--- |
| `git stash` | **Stashing** | Temporarily hides uncommitted work. | Sweeping papers into a drawer to clear desk. |
| `git stash list` | **Stashing** | Lists all stashed work saved in background. | Looking inside your desk drawer. |
| `git stash pop` | **Stashing** | Re-applies last stashed work and deletes stash. | Pulling items out of drawer back onto desk. |
| `git stash drop` | **Stashing** | Deletes specific stash without applying it. | Emptying the desk drawer into the trash. |
| `git cherry-pick <hash>` | **Porting** | Copies 1 specific commit from another branch. | Picking 1 exact apple off a different tree. |

---

## 5. Advanced History & Inspection

| Command | Category | What It Does | Real-World Analogy |
| :--- | :--- | :--- | :--- |
| `git diff` | **Diffing** | Shows exact unstaged line changes. | Comparing original paper with new edits. |
| `git diff --staged` | **Diffing** | Shows line changes staged for commit. | Inspecting staged photo lineup before shooting. |
| `git blame <file>` | **Auditing** | Shows who changed each line and when. | Looking at security footage of file edits. |
| `git bisect start` | **Debugging** | Starts binary search to find bug commit. | Playing higher/lower game to find broken code. |

---

## 6. Remote Repositories & GitHub

| Command | Category | What It Does | Real-World Analogy |
| :--- | :--- | :--- | :--- |
| `git remote -v` | **Remote** | Shows connected cloud URLs. | Checking Wi-Fi router connection details. |
| `git remote add origin <url>` | **Remote** | Connects local folder to GitHub URL. | Plugging ethernet cable into cloud server. |
| `git remote remove origin` | **Remote** | Removes remote connection link. | Unplugging ethernet cable. |
| `git push -u origin main` | **Syncing** | Uploads commits & sets tracking default. | Backing up photos to cloud storage. |
| `git fetch origin` | **Syncing** | Downloads remote updates WITHOUT merging. | Checking mail box without opening letters. |
| `git pull origin main` | **Syncing** | Fetches AND merges remote changes immediately. | Opening mail and acting on it right away. |
| `git clone <url>` | **Cloning** | Downloads full online repo to local PC. | Downloading a ZIP backup of a cloud Drive. |

---

## 7. GitHub Core Concepts & DevOps Workflows

* **Repositories (Repos):** Cloud folder hosting code, branches, and full history logs.
* **Pull Requests (PRs):** Formal proposal to review, test, and merge code changes into `main`.
* **Forks:** Personal server-side copy of someone else's repo under your own account.
* **Issues:** Interactive task board for tracking bug reports, feature tasks, and technical discussions.
* **GitHub Actions (CI/CD):** Automated workflows running tests, security scans, Docker builds, and cloud deployments on every commit or PR.

---

## 8. Quick Reference DevOps Matrix

| Task / Scenario | Primary Command |
| :--- | :--- |
| **Check current file state** | `git status` |
| **Stage all changes** | `git add .` |
| **Save snapshot locally** | `git commit -m "feat: setup app"` |
| **Push updates to GitHub** | `git push origin main` |
| **Fetch newest team code** | `git pull origin main` |
| **Start new feature safely** | `git switch -c feature/new-page` |
| **Emergency switch tasks** | `git stash` -> do hotfix -> `git stash pop` |
| **Safely undo bad deployment** | `git revert <broken-commit-hash>` |
| **Grab bug fix from dev** | `git cherry-pick <fix-commit-hash>` |
EOF
