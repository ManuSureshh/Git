# Git Commands
## Basic commands
1. Initialize the new Git repository
```
git init
```
2. Show the working directory status
```
git status
```
3. Add files to the staging area
- To add the specific file,
  ```
  git add filename
  ```
- To add all the files,
  ```
  git add .
  ```
4. Commit changes to the repository with a message.
```
git commit -m "Commit message"
```

5. Push commits to a remote repository.
```
git push origin main
```

6. Fetch and merge changes from the remote repository.
```
git pull origin main
```

## Branching and Merging
1. List, create, or delete branches.
```
git branch
```
```
git branch new-branch
```
```
git branch -d old-branch
```

2. Switch branches or restore working tree files.
- Switch to the main branch
  ```
  git checkout main
  ```
- Create and switch to a new branch
  ```
  git checkout -b new-branch
  ```
3. Merge a branch into the current branch.
   ```
   git merge new-branch
   ```

## Staching
1. Stash changes in the working directory.
```
git stash
```

2. List stashed changes
```
git stash list
```

3. Apply stashed changes.
```
git stash apply
```

4. Drop a stashed state.
```
git stash drop
```

## Viewing history
1. Show commit logs.
```
git log
```

2. Show changes between commits, commit and working tree, etc.
- Show unstaged changes
  ```
  git diff
  ```
  
- Show staged changes
  ```
  git diff --staged
  ```

3. Show various types of objects.
```
git show commit_hash
```

## Remote Repositories

1. Manage set of tracked repositories.
```
git remote -v
```

2. Add new Git remote
```
git remote add origin https://github.com/user/repo.git
```

4. Download objects and refs from another repository.
```
git fetch origin
```

6. Remove a remote
```
git remote rm origin
```

## Tagging

1. Create, list, delete, or verify a tag object.
- List tags
```
git tag
```

- Create an annotated tag
```
git tag -a v1.0 -m "Version 1.0"
```

- Delete a tag
```
git tag -d v1.0
```

2. Push tags to remote repository.
```
git push origin --tags
```

## Undoing Changes
1. Reset current HEAD to the specified state.
- Undo last commit, keep changes staged
```
git reset --soft HEAD~1
```

- Undo last commit, discard changes
```
git reset --hard HEAD~1
```

2. Revert a commit by creating a new commit.
```
git revert commit_hash
```

## Configuration
1. Get and set repository or global options.
```
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

## Advanced Commands
1. Apply the changes introduced by some existing commits.
```
git cherry-pick commit_hash
```

2. Reapply commits on top of another base tip.
```
git rebase main
```

3. Use binary search to find the commit that introduced a bug.
```
git bisect start
```
```
git bisect bad
```
```
git bisect good commit_hash
```

4. Show what revision and author last modified each line of a file.
```
git blame filename
```

5. Remove untracked files from the working directory.
- Force clean
```
git clean -f
```

- Remove directories
```
git clean -fd
```

6. Create custom git commands.
```
git config --global alias.co checkout
git config --global alias.ci commit
git config --global alias.st status
git config --global alias.br branch
```

   
