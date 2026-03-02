# Data Analysis Homework

**Authors:** A. Agung Prawira Negara & Nand Van Deun

Repository for data analysis assignments in physics and astronomy.

---

## Branch Structure

```
main              ← stable, final version only
├── branch-agung  ← Agung's working branch
└── branch-nand   ← Nand's working branch
```

> ⚠️ Never work directly on `main`!

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

Create your branch:
```bash
# Agung
git checkout -b branch-agung

# Nand
git checkout -b branch-nand
```

---

## Workflow: Every Time You Work

### 1. Always start by syncing with main
```bash
git checkout main
git pull origin main
git checkout branch-yourname
git merge main
```

### 2. Do your edits on the notebook, then save it

### 3. Clear notebook outputs before committing
In Jupyter: **Kernel → Restart & Clear Output**, then save.

### 4. Stage, commit, and push your work
```bash
git add .
git commit -m "describe what you changed"
git push origin branch-yourname
```

### 5. Open a Pull Request on GitHub
- Go to the repo page on GitHub
- Click **Compare & pull request**
- Write a short description of your changes
- Click **Create pull request**
- Notify your partner to review and merge it

### 6. After your PR is merged, sync up
```bash
git checkout main
git pull origin main
git checkout branch-yourname
git merge main
```

---

## ⚠️ If You Get a Conflict

This can happen when both of us edit the same file at the same time without knowing. Don't panic!

When you run `git pull origin main` and see:
```
CONFLICT (content): Merge conflict in notebook.ipynb
Automatic merge failed; fix conflicts and then commit the result.
```

You have two choices:

**Keep your local version:**
```bash
git checkout --ours HomeworkAssignment1_AAgungPrawiraNegara_NandVanDeun.ipynb
git add HomeworkAssignment1_AAgungPrawiraNegara_NandVanDeun.ipynb
git commit -m "resolve conflict, keep my version"
```

**Keep the GitHub (partner's) version:**
```bash
git checkout --theirs HomeworkAssignment1_AAgungPrawiraNegara_NandVanDeun.ipynb
git add HomeworkAssignment1_AAgungPrawiraNegara_NandVanDeun.ipynb
git commit -m "resolve conflict, keep partner's version"
```

> 💬 **Best practice: always communicate first!** Before starting work, let your partner know what you're working on so you don't edit the same cells at the same time.

---

## Quick Reference

| Action | Command |
|---|---|
| Check current branch | `git branch` |
| Check status | `git status` |
| Switch branch | `git checkout branch-name` |
| Pull latest main | `git pull origin main` |
| Merge main into your branch | `git merge main` |
| Stage all files | `git add .` |
| Commit | `git commit -m "message"` |
| Push | `git push origin branch-yourname` |

---

## Rules
- Each person works on their own branch (`branch-agung` or `branch-nand`)
- Never push directly to `main` — always go through a Pull Request
- Clear notebook outputs before committing
- Write clear commit messages so both of us can track what changed
- After a PR is merged, always sync your local branch with the updated main
