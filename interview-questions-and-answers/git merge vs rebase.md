### git merge vs git rebase

🔹 git merge

git merge combines changes from one branch into another by creating a merge commit.
It preserves complete history.

Real-time example:
Your team is working on a shared feature branch.
You merge it into main so that everyone can clearly see when the feature was integrated.

git checkout main
git merge feature-login

📌 Safe for shared branches
📌 History remains unchanged

🔹 git rebase

git rebase moves your commits on top of another branch, creating a clean, linear history by rewriting commits.

Real-time example:
You are working on a personal feature branch and want your commits to appear as if they were made after the latest main changes.

git checkout feature-login
git rebase main

📌 Clean commit history
📌 Should NOT be used on shared branches
