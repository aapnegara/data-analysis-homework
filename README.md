# Data Analysis Homework

## For Collaborators

Follow this guide to contribute to the repo without breaking anything.

---

## First Time Setup

Clone the repo to your machine:
```bash
git clone https://github.com/aapnegara/data-analysis-homework
cd data-analysis-homework
```

Set your identity (do this once):
```bash
git config --global user.email "your-github-email@example.com"
git config --global user.name "Your Name"
```

---

## Workflow: Every Time You Work

### 1. Always start by syncing with main
```bash
git checkout main
git pull origin main
```

### 2. Create your own branch before editing anything
```bash
git checkout -b branch-nand
```
> ⚠️⚠️⚠️ Never edit directly on `main`!

### 3. Do your edits on the notebook, then save it

### 4. Stage, commit, and push your work
```bash
git add .
git commit -m "describe what you changed"
git push origin branch-nand
```

### 5. Open a Pull Request on GitHub
- Go to the repo page on GitHub
- Click **Compare & pull request**
- Write a short description of your changes
- Click **Create pull request**

Then wait, I will review and merge it into main.

---

## Quick Reference

| Action | Command |
|---|---|
| Check status | `git status` |
| See your branch | `git branch` |
| Switch branch | `git checkout branch-name` |
| Pull latest main | `git pull origin main` |
| Stage all files | `git add .` |
| Commit | `git commit -m "message"` |
| Push | `git push origin branch-nand` |

---

## Rules
- Always work on `branch-nand`, not `main`
- Clear notebook outputs before committing (**Kernel → Restart & Clear Output**)
- Write clear commit messages so both of us can track and knows what is changed
