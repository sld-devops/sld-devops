# Sandis (sld-devops)

## Git/GitHub quick commands

### First-time setup
```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
``` 
### Start a repo locally
```bash
git init
git add .
git commit -m "Initial commit"
``` 
### Add new exercise
```bash
cd ~/bootdev-python-exercises
mkdir <exercise-name>
nano <exercise-name>/main.py

git add .
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
```
