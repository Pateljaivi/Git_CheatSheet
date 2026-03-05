# Git_CheatSheet - Git Commands

# 1. Git Configuration

Set up your Git identity before working with repositories.

```bash
git config --global user.name "Your Name"
```

Sets your Git username globally.

```bash
git config --global user.email "your@email.com"
```

Sets your Git email globally.

```bash
git config --local user.name "Your Name"
```

Sets username for the current repository.

```bash
git config --local user.email "your@email.com"
```

Sets email for the current repository.

---

# 2. Repository Setup

Initialize a new repository.

```bash
git init
```

Creates a `.git` directory and starts tracking the project.

Clone an existing repository.

```bash
git clone <repository_url>
```

Downloads a copy of a repository from GitHub.

---

# 3. Check Repository Status

```bash
git status
```

Shows:

* Untracked files
* Modified files
* Staged files
* Current branch

---

# 4. Add Files to Staging

Add a specific file.

```bash
git add file_name
```

Add multiple files.

```bash
git add file1 file2
```

Add all files.

```bash
git add .
```

Adds all modified and new files to staging.

---

# 5. Commit Changes

Create a commit with a message.

```bash
git commit -m "Commit message"
```

Add and commit tracked files together.

```bash
git commit -a -m "Message"
```

Edit the previous commit.

```bash
git commit --amend
```

---

# 6. Branch Management

View all branches.

```bash
git branch
```

Create a new branch.

```bash
git branch branch_name
```

Switch to another branch.

```bash
git switch branch_name
```

Create and switch to a new branch.

```bash
git switch -c branch_name
```

Delete a branch.

```bash
git branch -d branch_name
```

Force delete a branch.

```bash
git branch -D branch_name
```

---

# 7. Merge Branches

```bash
git merge branch_name
```

Merges another branch into the current branch.

Make sure you are on the branch where you want the merge to happen.

---

# 8. Git Diff

Show unstaged changes.

```bash
git diff
```

Show staged changes.

```bash
git diff --staged
```

Compare two branches.

```bash
git diff branch1 branch2
```

Compare two commits.

```bash
git diff commit1..commit2
```

---

# 9. Git Stash

Temporarily save changes.

```bash
git stash
```

View stash list.

```bash
git stash list
```

Apply stash without removing it.

```bash
git stash apply
```

Apply stash and remove it.

```bash
git stash pop
```

Delete a stash.

```bash
git stash drop stash@{0}
```

Clear all stashes.

```bash
git stash clear
```

---

# 10. Remote Repository

Check remote repositories.

```bash
git remote -v
```

Add remote repository.

```bash
git remote add origin https://github.com/username/repository.git
```

Remove remote repository.

```bash
git remote remove origin
```

---

# 11. Push, Pull & Fetch

Push changes to remote repository.

```bash
git push origin branch_name
```

Push and set upstream branch.

```bash
git push -u origin branch_name
```

Pull changes from remote.

```bash
git pull origin branch_name
```

Fetch remote changes.

```bash
git fetch
```

Fetch and remove deleted branches.

```bash
git fetch --prune
```

---

# 12. Git Rebase

Reapply commits on top of another branch.

```bash
git switch feature_branch
git rebase main
```

Abort rebase.

```bash
git rebase --abort
```

Continue after resolving conflicts.

```bash
git rebase --continue
```

Interactive rebase.

```bash
git rebase -i HEAD~3
```

---

# 13. Git Tags

Create a tag.

```bash
git tag v1.0
```

Create annotated tag.

```bash
git tag -a v1.0 -m "Version 1.0"
```

Push a tag.

```bash
git push origin v1.0
```

Push all tags.

```bash
git push origin --tags
```

---

# 14. GitFlow Commands

Initialize GitFlow.

```bash
git flow init
```

Start a feature branch.

```bash
git flow feature start feature_name
```

Finish feature.

```bash
git flow feature finish feature_name
```

Start a release.

```bash
git flow release start 1.0.0
```

Finish release.

```bash
git flow release finish 1.0.0
```

Start hotfix.

```bash
git flow hotfix start bug_name
```

Finish hotfix.

```bash
git flow hotfix finish bug_name
```

---




