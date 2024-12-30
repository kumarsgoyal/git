# Git Cheatsheet

### Getting Started

- Initialize a repository:  
  `git init`
- Clone a repository:  
  `git clone <repo-url>`

---

### Basic Commands

- Check the status of your repository:  
  `git status`
- Add files to the staging area:  
  `git add <file>`  
  `git add .` (Add all files)
- Commit changes:  
  `git commit -m "Your commit message"`
- View commit history:  
  `git log`

---

### Branching

- List all branches:  
  `git branch`
- Create a new branch:  
  `git branch <branch-name>`
- Switch to a branch:  
  `git checkout <branch-name>`  
  (or)  
  `git switch <branch-name>`
- Create and switch to a new branch:  
  `git checkout -b <branch-name>`  
  (or)  
  `git switch -c <branch-name>`

---

### Merging

- Merge a branch into the current branch:  
  `git merge <branch-name>`
- Abort a merge:  
  `git merge --abort`
- Resolve merge conflicts manually, then:  
  `git add <file>`  
  `git commit`

---

### Undoing Changes

- Unstage a file:  
  `git restore --staged <file>`
- Discard changes in a file:  
  `git restore <file>`
- Reset to the previous commit (soft):  
  `git reset --soft HEAD~1`
- Reset to the previous commit (hard):  
  `git reset --hard HEAD~1`

---

### Remote Repositories

- Add a remote:  
  `git remote add origin <repo-url>`
- View remotes:  
  `git remote -v`
- Push changes to a remote repository:  
  `git push origin <branch-name>`
- Pull changes from a remote repository:  
  `git pull origin <branch-name>`
- Fetch changes without merging:  
  `git fetch`

---

### Stashing

- Save changes for later:  
  `git stash`
- Apply the last stashed changes:  
  `git stash apply`
- List all stashed changes:  
  `git stash list`

---

### Tags

- Create a tag:  
  `git tag <tag-name>`
- Push tags to a remote:  
  `git push origin <tag-name>`

---

### Miscellaneous

- Show differences between commits:  
  `git diff`
- Show the last commit's changes:  
  `git show`
- Delete a branch:  
  `git branch -d <branch-name>`  
  `git branch -D <branch-name>` (force delete)
- Force push (use cautiously):  
  `git push --force`

---

### Helpful Tips

- View a visual representation of commits:  
  `git log --oneline --graph --all`
- Check who changed what in a file:  
  `git blame <file>`
- Undo the last commit (keep changes):  
  `git reset --soft HEAD~1`
