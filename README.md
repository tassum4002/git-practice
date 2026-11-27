# git-practice

A practice repository for learning core Git and GitHub workflows: branching, committing, opening Pull Requests, and stashing changes.

## Useful Git Workflow Notes

### 1. Branching
Create and switch to a new feature branch before making changes so `main` stays clean:
```bash
git checkout -b feature-update
# or in newer Git versions:
git switch -c feature-update
```

### 2. Staging and Committing
Inspect changes before staging, then write clear commit messages:
```bash
git status
git diff
git add README.md
git commit -m "Add Git workflow notes to README"
```

### 3. Pushing and Opening a Pull Request
Push the feature branch to the remote repository and open a Pull Request targeting `main`:
```bash
git push -u origin feature-update
```

### 4. Stashing Uncommitted Changes
Temporarily save uncommitted edits without committing them:
```bash
git stash
git stash list
git stash pop
```
Note: Stashed changes are stored in a stack (`stash@{0}`, `stash@{1}`, ...) and can be popped onto the current working branch.
