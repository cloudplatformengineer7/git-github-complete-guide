# Branching and Merging in Git

Branching allows developers to work on features independently, while merging combines changes back into a single codebase.  
This is one of Git’s most powerful features for collaborative development.

---

## 1. What is a Branch?

A branch is a **separate line of development**.

- The default branch is usually master in git, whereas main in GitHub
- Each branch has its own commit history
- Changes in one branch do not affect others

📌 Branching enables **safe experimentation and parallel development**.

---

## 2. Creating and Viewing Branches

### List All Branches

git branch

Create a New Branch

git branch feature-login

Switch to a Branch

git checkout feature-login

Create and Switch in One Command

git checkout -b feature-login

3. Working with Branches (Example)
   
You are adding a login feature:

git checkout -b feature-login

Make code changes and commit:

git add .
git commit -m "Add login functionality"

The main branch remains unchanged while you work on feature-login.

4. Merging Branches

Merging combines changes from one branch into another.

Basic Merge

First, switch to the target branch:

git checkout main
Merge the feature branch:

git merge feature-login

📌 This brings all changes from feature-login into main.

5. Types of Merges

Fast-Forward Merge

Occurs when the target branch has no new commits.
Git simply moves the pointer forward
No merge commit created

Three-Way Merge

Occurs when both branches have new commits.
Git creates a merge commit
Preserves both histories

7. Merge Conflicts
   
A merge conflict occurs when:
The same file is modified in both branches
Git cannot decide which change to keep

Resolving Conflicts

Open the conflicted file
Choose the correct changes
Remove conflict markers
Commit the resolved changes

git add .
git commit -m "Resolve merge conflict"

9. Deleting Branches
    
Delete a local branch after merging:

git branch -d feature-login

Force delete (not recommended):

git branch -D feature-login

11. Best Practices

Create a branch for every feature or bug fix
Keep branches short-lived
Merge frequently to avoid conflicts
Delete branches after successful merge

13. Summary

Branches isolate development work
Merging combines changes safely
Conflicts are normal and manageable
Branching enables scalable team collaboration

Branching and merging are core Git workflows used in all modern software projects.
