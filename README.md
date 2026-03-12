# Github_practice

A repository for practicing and revising common GitHub (Git) commands.

---

## 🔧 Git Configuration

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --list
```

---

## 📁 Repository Setup

```bash
# Initialize a new local repository
git init

# Clone an existing repository
git clone <repository-url>
```

---

## 📄 Staging & Committing

```bash
# Check the status of your working directory
git status

# Add a specific file to staging
git add <file>

# Add all changes to staging
git add .

# Commit staged changes with a message
git commit -m "Your commit message"

# Add and commit in one step (only for tracked files)
git commit -am "Your commit message"
```

---

## 🌿 Branching

```bash
# List all local branches
git branch

# Create a new branch
git branch <branch-name>

# Switch to a branch
git checkout <branch-name>

# Create and switch to a new branch
git checkout -b <branch-name>

# Delete a branch
git branch -d <branch-name>
```

---

## 🔀 Merging & Rebasing

```bash
# Merge a branch into the current branch
git merge <branch-name>

# Rebase current branch onto another
git rebase <branch-name>
```

---

## 🌐 Remote Repositories

```bash
# View remote connections
git remote -v

# Add a remote
git remote add origin <repository-url>

# Fetch changes from remote
git fetch origin

# Pull latest changes from remote
git pull origin <branch-name>

# Push local changes to remote
git push origin <branch-name>

# Push and set upstream tracking
git push -u origin <branch-name>
```

---

## 📜 Viewing History

```bash
# Show commit history
git log

# Show compact one-line log
git log --oneline

# Show changes for a specific commit
git show <commit-hash>

# Show differences between working directory and staging
git diff

# Show differences between staging and last commit
git diff --staged
```

---

## ↩️ Undoing Changes

```bash
# Unstage a file (keep changes in working directory)
git restore --staged <file>

# Discard changes in working directory
git restore <file>

# Amend the last commit message
git commit --amend -m "New commit message"

# Revert a commit (creates a new undo commit)
git revert <commit-hash>

# Reset to a previous commit (use with caution)
git reset --hard <commit-hash>
```

---

## 🏷️ Tags

```bash
# List all tags
git tag

# Create a lightweight tag
git tag <tag-name>

# Create an annotated tag
git tag -a <tag-name> -m "Tag message"

# Push a tag to remote
git push origin <tag-name>
```

---

## 🤝 Pull Requests (GitHub Workflow)

1. Fork or clone the repository
2. Create a new feature branch: `git checkout -b feature/my-feature`
3. Make changes and commit: `git commit -m "Add my feature"`
4. Push to your fork/remote: `git push origin feature/my-feature`
5. Open a Pull Request on GitHub

---

## 💡 Useful Tips

```bash
# Save work temporarily without committing
git stash

# Re-apply stashed changes
git stash pop

# See all stashes
git stash list

# Clean untracked files (dry-run)
git clean -n

# Show a visual branch graph
git log --oneline --graph --all
```
