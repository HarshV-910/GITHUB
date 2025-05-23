# Overview of Git Branches, Conflicts, and Solutions

## What are Git Branches?
Git branches are a way to work on different versions of a repository simultaneously. A branch is essentially a pointer to a specific commit in the repository. The default branch in Git is usually called `main` or `master`. Developers create branches to isolate their work, allowing them to experiment or develop features without affecting the main codebase.

### Key Commands for Branches:
- Create a new branch: ```git branch <branch-name>```
- To show all branches: ```git branch```

- Switch to a branch: ```git checkout <branch-name>``` or ```git switch <branch-name>```

- Create and switch to a branch: ```git checkout -b <branch-name>``` or ```git switch -c <branch-name>```

- Merge a branch (we are should at main branch to merge): ```git merge <branch-name>```

- Delete a branch: ```git branch -d <branch-name>```

---

## What are Branch Conflicts?
Branch conflicts occur when Git cannot automatically merge changes from one branch into another. This usually happens when the same lines of code are modified in both branches or when changes are made to the same file in incompatible ways.
ex: we have file with 20 lines, now we are creating 2 sub-branch for sharing now first person A commit changes and now original file become of 25 lines and second person have also have changed 20 line file to 25 line. now when second person will trying to commit at time confilct occure that which changes git should have to take. original 25 line or 25 lines given by second person. to solve this we have like 3 solutions:
1) incoming change 
2) current change 
3) both merge by union

##When we are merging conflicted file at that time we got 3 option which above given and 1 compare option and then we can select any option for our final changes at main branch.

### Types of Conflicts:
1. **Merge Conflicts**: Occur during a ```git merge``` when Git cannot automatically resolve differences between branches.
2. **Rebase Conflicts**: Occur during a ```git rebase``` when applying commits from one branch onto another.

---

## Types of Merges:
1. **Three-Way Merge**:
    - A three-way merge occurs when Git uses three commits to generate the merge: the two branch tips and their common ancestor.
    - This is the most common type of merge when branches have diverged.
    - Command: ```git merge <branch-name>```

2. **Fast-Forward Merge**:
    - A fast-forward merge occurs when the branch being merged has no additional commits compared to the current branch.
    - In this case, Git simply moves the branch pointer forward to the latest commit.
    - Command: ```git merge --ff <branch-name>``` (default behavior)

3. **No Fast-Forward Merge**:
    - This type of merge creates a merge commit even if a fast-forward merge is possible. It is useful for preserving the branch history.
    - Command: ```git merge --no-ff <branch-name>```

---

## Solutions to Resolve Conflicts:

1. **Complete the Merge/Rebase**:
    - For a merge: Run ```git commit``` to complete the merge.
    - For a rebase: Run ```git rebase --continue``` to continue the rebase process.

2. **Abort the Operation (if needed)**:
    - If you want to cancel the merge or rebase, use:
      - ```git merge --abort```
      - ```git rebase --abort```

---

##To delete branch: ```git branch -d <branch_name>```