# 🔗 Git & GitHub – Remote Repository Commands

This section explains how a **local Git repository communicates with a remote repository (GitHub)**.
These commands are used daily by developers and DevOps engineers.

##  Linking Local Repository to Remote Repository

### Command:

git remote add origin <repo-url>

### Purpose:

Links your **local repository** to a **central GitHub repository**.

### Example:

git remote add origin https://github.com/username/project.git

📌 origin is the default name for the remote repository.

##  View Linked Remote Repositories

### Command:

git remote -v

### Purpose:

Displays the **remote repository URLs** linked to your local repository.

### Output Example:


origin  https://github.com/username/project.git (fetch)
origin  https://github.com/username/project.git (push)

##  Push Code from Local to GitHub

### Command:

git push -u origin <branch-name>

### Purpose:

Pushes code from **local branch** to **GitHub** and sets upstream tracking.

### Example:

git push -u origin main

##  Push Code to Multiple Branches

### Command:

git push origin branch-1 branch-2

### Purpose:

Pushes changes to **multiple branches** at the same time.

##  Push All Local Branches to GitHub

### Command:

git push -u origin --all

### Purpose:

Pushes **all local branches** to the remote repository.

##  Clone a Remote Repository

### Command:

git clone <repo-url>

### Purpose:

Downloads a **remote GitHub repository** to your local system.

### Example:

git clone https://github.com/username/project.

##  Pull Changes from GitHub to Local

### Command:

git pull origin <branch-name>


### Purpose:

Fetches changes from GitHub **and merges them** into the local branch.

### Example:

git pull origin main

📌 `git pull = git fetch + git merge`

##  Fetch Changes from Remote Repository

### Command:

git fetch <branch-name>

### Purpose:

Downloads changes from GitHub **without merging** them.

### Example:

git fetch main

##  Fetch All Branches from GitHub

### Command:

git fetch --all

### Purpose:

Fetches updates from **all remote branches**.

## 🔍 Difference: git fetch vs git pull

| Command   | Behavior                   |
| --------- | -------------------------- |
| git fetch | Downloads changes only     |
| git pull  | Downloads + merges changes |

---

## Merge Remote Branch into Local Branch

### Command:

git merge origin/<branch-name>

### Purpose:

Merges fetched remote branch changes into the current local branch.

### Example:

git merge origin/main

##  Delete a Branch from GitHub (Remote)

### Command

git push origin --delete <branch-name>
Purpose:

Deletes a branch from the remote GitHub repository.

Example:
git push origin --delete feature-login

Remove Remote Repository Link

Command:
git remote rm origin
Purpose:

Unlinks the local repository from GitHub.

Rename a Remote Repository

Command:
git remote rename old-name new-name
Purpose:

Renames an existing remote reference.

Example:
git remote rename origin upstream
