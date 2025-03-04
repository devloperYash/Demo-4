# Git & GitHub Guide

## Introduction
This guide will help you get started with Git and GitHub, covering installation, basic Git commands, and collaboration workflows.

---
## 1. Installation

### Windows:
- Download and install Git from [git-scm.com](https://git-scm.com/)
- Use Git Bash or Command Prompt to execute Git commands

### MacOS:
- Install Git using Homebrew:
  ```sh
  brew install git
  ```

### Linux (Debian-based):
- Install Git using:
  ```sh
  sudo apt update && sudo apt install git
  ```

Verify installation:
```sh
git --version
```
---

## 2. Setting Up Git

Configure your user information:
```sh
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

Check your configuration:
```sh
git config --list
```
---

## 3. Basic Git Commands

### Initialize a Git Repository
```sh
git init
```

### Clone a Repository
```sh
git clone https://github.com/username/repository.git
```

### Check Repository Status
```sh
git status
```

### Add Files to Staging Area
```sh
git add filename
# or add all files
 git add .
```

### Commit Changes
```sh
git commit -m "Your commit message"
```

### View Commit History
```sh
git log
```

### Push Changes to GitHub
```sh
git push origin main
```

### Pull Latest Changes from Remote Repository
```sh
git pull origin main
```

### Create a New Branch
```sh
git branch branch-name
```

### Switch to a Branch
```sh
git checkout branch-name
```

### Merge a Branch
```sh
git merge branch-name
```

### Delete a Branch
```sh
git branch -d branch-name
```
---

## 4. Working with GitHub

### Create a New Repository on GitHub
1. Go to [GitHub](https://github.com/) and log in.
2. Click on `New Repository`.
3. Name your repository and click `Create`.
4. Follow the provided instructions to connect your local repository.

### Add a Remote Repository
```sh
git remote add origin https://github.com/username/repository.git
```

### Forking a Repository
- Navigate to a repository on GitHub and click `Fork`.
- Clone your forked repository:
```sh
git clone https://github.com/your-username/forked-repo.git
```

### Creating a Pull Request (PR)
1. Push changes to your branch.
2. Go to the original repository on GitHub.
3. Click `Pull Requests > New Pull Request`.
4. Select your branch and describe the changes.
5. Click `Create Pull Request`.

---
## 5. Collaboration Workflow

### Step 1: Clone the Repository
```sh
git clone https://github.com/username/repository.git
```

### Step 2: Create a Feature Branch
```sh
git checkout -b feature-branch
```

### Step 3: Make Changes and Commit
```sh
git add .
git commit -m "Added a new feature"
```

### Step 4: Push Changes
```sh
git push origin feature-branch
```

### Step 5: Create a Pull Request
- Open GitHub and navigate to your repository.
- Click `Pull Requests` and create a new PR.
- Request a review and merge when approved.

---
## 6. Undoing Changes

### Undo Last Commit (Keep Changes)
```sh
git reset --soft HEAD~1
```

### Undo Last Commit (Remove Changes)
```sh
git reset --hard HEAD~1
```

### Revert a Commit
```sh
git revert commit-id
```

---
## Conclusion
This guide covers the basics of Git and GitHub. Keep practicing to master version control!
