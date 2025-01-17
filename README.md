# GIT-Commands
These are the most used commands in Git

----

# Set up your Git username globally for all repositories
git config --global user.name "Your Name"

# Set up your Git email globally for all repositories
git config --global user.email "your.email@example.com"

# Check your current Git configuration
git config --list

# Initialize a new Git repository in the current directory
git init

# Clone an existing repository from a URL
git clone <repository-url>

# Check the status of your working directory (untracked/modified files, etc.)
git status

# Add a specific file to the staging area
git add <file>

# Add all files in the current directory to the staging area
git add .

# Commit staged changes with a descriptive message
git commit -m "Commit message"

# Remove a specific file from the working directory and stage the removal
git rm <file>

# Create a new branch with a given name
git branch <branch-name>

# Switch to an existing branch
git checkout <branch-name>

# Create and switch to a new branch simultaneously
git checkout -b <branch-name>

# List all branches in the repository
git branch

# Delete a specific branch
git branch -d <branch-name>

# View the configured remote repositories and their URLs
git remote -v

# Add a new remote repository and name it 'origin'
git remote add origin <repository-url>

# Push the current branch to the remote repository
git push origin <branch-name>

# Pull changes from a specific branch in the remote repository
git pull origin <branch-name>

# Fetch updates from the remote repository without merging
git fetch

# Discard changes in a specific file and restore it to the last committed state
git checkout -- <file>

# Unstage a file but keep its changes in the working directory
git reset <file>

# Undo the last commit but keep the changes in the staging area
git reset --soft HEAD~1

# Undo the last commit and remove all changes from the working directory
git reset --hard HEAD~1

# View the commit history in detail
git log

# View the commit history as a single line per commit
git log --oneline

# Show changes made in a specific commit
git show <commit-hash>

# Merge a specified branch into the current branch
git merge <branch-name>

# Reapply commits from a different branch onto the current branch
git rebase <branch-name>

# Save current changes temporarily without committing
git stash

# List all stashed changes
git stash list

# Apply the latest stash without removing it from the stash list
git stash apply

# Apply the latest stash and remove it from the stash list
git stash pop
