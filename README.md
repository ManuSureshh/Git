# Git
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
2. Show changes between commits, commit and working tree, etc.
- Show unstaged changes
- Show staged changes
3. Show various types of objects.
4. Manage set of tracked repositories.
5. Download objects and refs from another repository.
6. Remove a remote

## Tagging 
1. Create, list, delete, or verify a tag object.
- List tags
- Create an annotated tag
- Delete a tag

2. Push tags to remote repository.

## Undoing Changes
1. Reset current HEAD to the specified state.
- Undo last commit, keep changes staged
- Undo last commit, discard changes

2. Revert a commit by creating a new commit.

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
3. Use binary search to find the commit that introduced a bug.
4. Show what revision and author last modified each line of a file.
5. Remove untracked files from the working directory.
6. Create custom git commands.
```
git config --global alias.co checkout
git config --global alias.ci commit
git config --global alias.st status
git config --global alias.br branch
```

   
