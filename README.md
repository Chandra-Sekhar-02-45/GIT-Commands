# GIT-Commands

These are the most used commands in Git:

---

### Set up your Git username globally for all repositories
```bash
git config --global user.name "Your Name"
```

### Set up your Git email globally for all repositories
```bash
git config --global user.email "your.email@example.com"
```

### Check your current Git configuration
```bash
git config --list
```

### Initialize a new Git repository in the current directory
```bash
git init
```

### Clone an existing repository from a URL
```bash
git clone <repository-url>
```

### Check the status of your working directory (untracked/modified files, etc.)
```bash
git status
```

### Add a specific file to the staging area
```bash
git add <file>
```

### Add all files in the current directory to the staging area
```bash
git add .
```

### Commit staged changes with a descriptive message
```bash
git commit -m "Commit message"
```

### Remove a specific file from the working directory and stage the removal
```bash
git rm <file>
```

### Create a new branch with a given name
```bash
git branch <branch-name>
```

### Switch to an existing branch
```bash
git checkout <branch-name>
```

### Create and switch to a new branch simultaneously
```bash
git checkout -b <branch-name>
```

### List all branches in the repository
```bash
git branch
```

### Delete a specific branch
```bash
git branch -d <branch-name>
```

### View the configured remote repositories and their URLs
```bash
git remote -v
```

### Add a new remote repository and name it 'origin'
```bash
git remote add origin <repository-url>
```

### Push the current branch to the remote repository
```bash
git push origin <branch-name>
```

### Pull changes from a specific branch in the remote repository
```bash
git pull origin <branch-name>
```

### Fetch updates from the remote repository without merging
```bash
git fetch
```

### Discard changes in a specific file and restore it to the last committed state
```bash
git checkout -- <file>
```

### Unstage a file but keep its changes in the working directory
```bash
git reset <file>
```

### Undo the last commit but keep the changes in the staging area
```bash
git reset --soft HEAD~1
```

### Undo the last commit and remove all changes from the working directory
```bash
git reset --hard HEAD~1
```

### View the commit history in detail
```bash
git log
```

### View the commit history as a single line per commit
```bash
git log --oneline
```

### Show changes made in a specific commit
```bash
git show <commit-hash>
```

### Merge a specified branch into the current branch
```bash
git merge <branch-name>
```

### Reapply commits from a different branch onto the current branch
```bash
git rebase <branch-name>
```

### Save current changes temporarily without committing
```bash
git stash
```

### List all stashed changes
```bash
git stash list
```

### Apply the latest stash without removing it from the stash list
```bash
git stash apply
```

### Apply the latest stash and remove it from the stash list
```bash
git stash pop
```

---

## Fork Workflow

### Step 1: Fork the repository
- Go to the repository page on GitHub (or your hosting platform) and click the "Fork" button.
- This creates a copy of the repository in your account.

### Step 2: Clone your forked repository to your local system
```bash
git clone <your-forked-repository-url>
```

### Step 3: Add the original repository (upstream) as a remote
```bash
git remote add upstream <original-repository-url>
```

### Step 4: Verify the remotes to confirm 'origin' and 'upstream' are set correctly
```bash
git remote -v
```

### Step 5: Fetch changes from the original repository to stay updated
```bash
git fetch upstream
```

### Step 6: Merge the updates from the original repository into your local branch
```bash
git merge upstream/<branch-name>
```

### Step 7: Push your changes back to your forked repository if needed
```bash
git push origin <branch-name>
