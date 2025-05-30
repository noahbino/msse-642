# Git Command Line Activities

## Configuration

### Set user name and email (global)
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

### Set core editor
git config --global core.editor "code --wait"

### View global and local config
git config --global --list
git config --local --list

### Create a new local repo
mkdir my-new-repo
cd my-new-repo
git init

### Clone a public repo 
git clone https://github.com/octocat/Hello-World.git

### View repo status 
git status

### Stage changes 
git add filename.txt

### Commit changes 
git commit -m "Added filename.txt with initial content"

### Example .gitignore
# .gitignore
node_modules/
.env
*.log

### Delete files using git
git rm oldfile.txt
git commit -m "Removed oldfile.txt"

## Working With Remote 

### View remote repo 
git remote -v

### Use git fetch
git fetch

### pull 
git pull

### Make local changes and push 
echo "Hello Git" >> hello.txt
git add hello.txt
git commit -m "Added hello.txt"
git push origin main

## Branches 

### View Branches 
git branch         # local
git branch -r      # remote

### Create new branch 
git branch         # before
git checkout -b feature-branch
git branch         # after

### switch branches 
git checkout feature-branch
# OR
git switch feature-branch

### delete local branch
git branch -d feature-branch   # will fail if unmerged
git branch -D feature-branch   # forces delete

git branch     # confirm it's gone