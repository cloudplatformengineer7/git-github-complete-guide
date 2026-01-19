# Understanding Git: Areas & File Lifecycle

Git tracks changes in your project through **three main areas**. 

Think of it like moving your files through different “zones” before they become part of your project history.

---

## 🖥 Working Directory

- This is where you edit your files.  
- Git knows these files exist, but it doesn’t track changes yet.  
- Example: You create a new file app.py – Git sees it as new, but it’s untracked.

---

## 📝 Staging Area (Index)

- This is your draft zone.  
- Files here are **prepared for commit.  
- You move changes here using git add.  
- Think of it like telling Git: “These changes are ready to be saved.”

---

## 💾 Local Repository

- This is where your commits live permanently.  
- Every commit is a snapshot of your project at that moment.  
- Example: git commit -m "Add login feature" saves all staged changes in your local repo.

---

## 🔄 Git File Lifecycle

Every file in Git goes through **four** states:

1. Untracked – New file, Git doesn’t track it yet  
2. Staged – Changes added with git add, ready for commit  
3. Committed – Changes saved permanently in the local repository  
4. Modified – Tracked file changed but not yet staged  

---

📌 **Quick Tip:**  
> Edit → Stage → Commit → Repeat  

This simple flow is the core of working with Git.
