# Sandis (sld-devops)
## About me
I’m focusing on backend/devops fundamentals.
This repo documents my journey through Boot.dev courses, challenges, and small practice projects to build consistency and problem‑solving skills.
Current stack: Python • Linux CLI • Git/GitHub • small automation scripts

**Now:** 
• Python 
• Linux CLI 
• Git/GitHub 
• small automation scripts
## Git/GitHub quick commands

### First-time setup
```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
``` 
### Start a repo locally
```bash
git init
git branch -M main
git add .
git commit -m "Initial commit"
``` 
### Add new exercise
```bash
mkdir -p ~/repository-name # if new repo created
cd ~/repository-name
mkdir <exercise-name>
nano <exercise-name>/main.py # paste code, save (Ctrl+O, Enter), exit (Ctrl+X)

git add <exercise-name>
git commit -m "Add <exercise-name> exercise"
git push
```
### Connect to GitHub + push
```bash
git branch -M main
git remote add origin https://github.com/<user>/<repo>.git
git push -u origin main
```
### Daily workflow
```bash
git status
git add .
git commit -m "Describe change"
git push
```
### Sync before you push (if GitHub has new commits)
```bash
git pull --rebase
git push
```
### New branch workflow
```bash
git switch -c feature-name
git push -u origin feature-name
```
### Create a new folder + file (Ubuntu)
```bash
mkdir my-exercise
nano my-exercise/main.py
```
### View history
```bash
git log --oneline --decorate --graph --all
```
### Undo (common)
```bash
git restore <file>          # discard unstaged changes
git restore --staged <file> # unstage
```
### Check remotes/branch
```bash
git remote -v
git branch
```
### Clone an existing repo
```bash
git clone https://github.com/<user>/<repo>.git
cd repo-name
git remote add origin git@github.com:<user>/<repo>.git
git diff
```
