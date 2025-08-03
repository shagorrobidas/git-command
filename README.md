# Common Git Commands Reference

## Configuration
-  Set your Git username globally.
```
git config --global user.name "Your Name"
``` 

 - Set your Git email globally.
 ```
 git config --global user.email "you@example.com"
```  

 - Show all Git config settings.
```
git config --list
```  

---

## Repository Initialization
-  Initialize a new Git repository in the current directory.
```
git init
```  

 - Clone an existing repository from a URL.
```
git clone <repository-url>
```  

---

## Basic Workflow
-  Show the status of changes in the working directory.
```
git status
``` 

 - Stage file(s) for commit.
```
git add <file>
```

 - Stage all changed files.
```
git add .
```

 - Commit staged changes with a message.
```
git commit -m "Commit message"
```

 - Stage and commit tracked files with a message.
``` 
git commit -am "Commit message"
```

 - Show unstaged changes.
``` 
git diff
```  

 - Show staged changes.
``` 
git diff --staged
``` 

---

## Branching and Merging
 - List all branches.
```
git branch
```

 - Create a new branch.
```
git branch <branch-name>
```

 - Switch to a branch.
``` 
git checkout <branch-name>
```

 - Create and switch to a new branch.
``` 
git checkout -b <branch-name>
```

 - Merge specified branch into current branch.
``` 
git merge <branch-name>
```

 - Delete a branch.
``` 
git branch -d <branch-name>
```

---

## Remote Repositories
 - Show remote repository URLs.
```
 git remote -v
```

 - Add a remote repository.
``` 
git remote add origin <url>
```

 - Fetch changes from remote without merging.
``` 
git fetch
```
 - Fetch and merge changes from remote.

``` 
git pull
```

 - Push commits to remote repository.
```
git push
```

-  Push branch and set upstream tracking.
```
git push -u origin <branch-name>
``` 

---

## Undo and Reset
 - Unstage a file.
``` 
git reset <file>
```

 - Reset working directory and staging area to last commit (WARNING: irreversible).
```
git reset --hard
```

-  Create a new commit that undoes the changes from a previous commit.
```
git revert <commit>
```

---

## Logs and History
 - Show commit history.
```
git log
```

 - Show compact commit history.
```
git log --oneline
```

 - Show details about a specific commit.
```  
git show <commit>
``` 

---

## Tags
 - List tags.
```  
git tag
``` 

-  Create a new tag.
``` 
git tag <tag-name>
``` 

 - Push tag to remote.
``` 
git push origin <tag-name>
``` 

---

## Stashing
 - Save current changes temporarily.
``` 
git stash
``` 

 - List stashed changes.
``` 
git stash list
``` 

-  Re-apply stashed changes.
``` 
git stash apply
``` 

---

## Others
-  Remove untracked files.
``` 
git clean -f
``` 

-  Show who last modified each line in a file.
```
 git blame <file>
``` 

 - Remove a remote.
```
git remote remove <name>
``` 

---

**Note:** Replace `<branch-name>`, `<file>`, `<commit>`, `<repository-url>`, and `<tag-name>` with your actual branch names, file names, commit hashes, URLs, or tag names.

