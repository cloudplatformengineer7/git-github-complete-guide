This document covers all essential Git commands required to work with repositories, track changes, and manage code versions effectively.

1. Create or Download a Repository
   
 Initialize a New Repository

 Creates a new Git repository in the current directory:

  git init

2. Clone an Existing Repository

 Downloads a remote repository to your local system:

 git clone <repository-url>

3. Check Repository Status
   
 Displays the current state of files:

 git status

 Shows:

Untracked files
Modified files
Staged files

4. Add Files to Staging Area
   
 Add a specific file:

 git add file.txt

 Add all files:

 git add .

📌 Staging prepares files for versioning.

5. Commit Changes
   
 Save staged changes to the local repository:

 git commit -m "Write a meaningful commit message"

📌 A commit represents a snapshot of the project.

6. View File Differences
   
 Check unstaged changes:

 git diff

 Check staged changes:

 git diff --staged

7. Remove Files
   
 Remove file from Git and working directory:

 git rm file.txt

 Remove file only from tracking:

 git rm --cached file.txt

8. Rename or Move Files

 Rename or move a file:

 git mv old_name.txt new_name.txt

9. Undo Changes
    
 Discard local file changes:

 git checkout -- file.txt

 Unstage a file

 git restore --staged file.txt


10.Summary

 git init → create repository
 
 git clone → download repository
 
 git add → stage changes
 
 git commit → save changes
 
 git status → check state
 
 git log → view history

These commands form the foundation of Git usage.
