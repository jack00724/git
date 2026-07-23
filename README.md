cat << 'EOF' > README.md
# 🚀 My Git & GitHub Cheat Sheet

A quick reference guide for essential Git commands and GitHub concepts.

---

## 🛠️ Essential Git Commands Workflow

| Command | Category | What It Does | Real-World Analogy |
| :--- | :--- | :--- | :--- |
| `git config --global user.name "..."` | **Setup** | Sets your username and email for all your Git commits. | Writing your name on your notebook cover. |
| `git init` | **Setup** | Turns the current folder into a brand-new Git repository. | Buying a fresh journal and opening page 1. |
| `git status` | **Inspection** | Shows untracked files, staged changes, and current branch state. | Looking at your desk to see what needs organizing. |
| `git add ` | **Staging** | Moves file changes into the **staging area** to get ready for a save. | Lining people up in front of the camera before taking a picture. |
| `git commit -m "message"` | **Saving** | Saves a permanent snapshot of staged files with a descriptive message. | Clicking the shutter button to take the photo and saving it. |
| `git log --oneline` | **Inspection** | Displays a concise list of past commits (your project's history). | Flipping through your photo album to view past saves. |
| `git branch -M main` | **Branching** | Renames your primary local working branch to `main`. | Labeling the main trunk of your project tree. |
| `git remote add origin ` | **Remote** | Links your local folder to a remote repository on GitHub. | Plugging in a network cable to connect your laptop to the cloud. |
| `git remote -v` | **Inspection** | Checks which GitHub URLs your local repository is currently linked to. | Checking your Wi-Fi connection settings. |
| `git remote remove origin` | **Remote** | Removes the linked GitHub repository URL from your local setup. | Unplugging that network cable. |
| `git push -u origin main` | **Syncing** | Uploads your local commits to GitHub and sets up future tracking. | Backing up your local files to Google Drive/Cloud. |

---

## ☁️ GitHub Core Concepts

* **Repositories (Repos):** Your project's cloud folder hosting code and commit history.
* **Pull Requests (PRs):** Proposed changes submitted for team review before merging into `main`.
* **Forks:** A personal copy of someone else's repo under your own GitHub account.
* **Issues:** A board for tracking tasks, bug reports, and discussions.
* **Actions:** Automated tasks (CI/CD) that run tests or deployments automatically.
EOF
