# 🛠️ Git Cheat Sheet

A comprehensive guide to the most commonly used Git commands.

---

## 🚀 Getting Started

Initialize a new local repository or clone an existing one.

* **Initialize a repository**
  ```bash
  git init
  ```
* **Clone a remote repository**
  ```bash
  git clone <repository-url>
  ```

---

## 📝 Making Changes

Track, stage, and save your file modifications.

* **Check repository status**
  ```bash
  git status
  ```
* **Stage a specific file**
  ```bash
  git add <file-name>
  ```
* **Stage all changes**
  ```bash
  git add .
  ```
* **Commit staged changes**
  ```bash
  git commit -m "Your commit message"
  ```
* **Commit all tracked files directly (skips git add)**
  ```bash
  git commit -am "Your commit message"
  ```

---

## 🌿 Branching & Merging

Manage isolated lines of development.

* **List all local branches**
  ```bash
  git branch
  ```
* **Create a new branch**
  ```bash
  git branch <branch-name>
  ```
* **Switch to a branch**
  ```bash
  git checkout <branch-name>
  ```
* **Create and switch to a new branch instantly**
  ```bash
  git checkout -b <branch-name>
  ```
* **Merge a branch into the current active branch**
  ```bash
  git merge <branch-name>
  ```
* **Delete a local branch**
  ```bash
  git branch -d <branch-name>
  ```

---

## 🌍 Remote Repositories

Sync your local work with online platforms like GitHub or GitLab.

* **View connected remote repositories**
  ```bash
  git remote -v
  ```
* **Link a local repository to a remote server**
  ```bash
  git remote add origin <repository-url>
  ```
* **Download changes from remote without merging**
  ```bash
  git fetch
  ```
* **Fetch and merge remote changes into your active branch**
  ```bash
  git pull
  ```
* **Upload local commits to a remote repository**
  ```bash
  git push origin <branch-name>
  ```

---

## 🔍 History & Inspection

Review project updates, commit timelines, and differences.

* **View commit history**
  ```bash
  git log
  ```
* **View simplified, one-line commit history**
  ```bash
  git log --oneline
  ```
* **Show changes between working directory and last commit**
  ```bash
  git diff
  ```

---

## 🧹 Undo & Reset

Fix mistakes by reverting or changing history.

* **Discard changes in a specific file**
  ```bash
  git checkout -- <file-name>
  ```
* **Unstage a file (keep local modifications)**
  ```bash
  git reset HEAD <file-name>
  ```
* **Reset repository to a specific commit (safe: preserves files)**
  ```bash
  git reset --soft <commit-hash>
  ```
* **Reset repository completely (danger: destroys unsaved work)**
  ```bash
  git reset --hard <commit-hash>
  ```
