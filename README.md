To control versioning in GitHub, you need to understand Git and how it integrates with GitHub. Here are key concepts and commands to manage version control effectively:

### **1. Initialize a Git Repository**
If your project is not already a Git repository, initialize it:
```sh
git init
```

### **2. Clone a Repository**
If you need to work on an existing project hosted on GitHub:
```sh
git clone <repository-url>
```

### **3. Check Status**
To check which files are modified or staged:
```sh
git status
```

### **4. Stage Changes**
To add specific files to staging:
```sh
git add <filename>
```
To add all modified files:
```sh
git add .
```

### **5. Commit Changes**
To commit staged changes with a message:
```sh
git commit -m "Your commit message"
```

### **6. Push Changes to GitHub**
To push local commits to a remote branch:
```sh
git push origin <branch-name>
```
For the main branch, it’s usually:
```sh
git push origin main
```

### **7. Pull Latest Changes**
To update your local branch with the latest changes from GitHub:
```sh
git pull origin <branch-name>
```

### **8. Create and Switch Branches**
To create a new branch:
```sh
git branch <new-branch-name>
```
To switch to that branch:
```sh
git checkout <new-branch-name>
```
Or use:
```sh
git switch <new-branch-name>
```

### **9. Merge Branches**
To merge a branch into the current branch:
```sh
git merge <branch-name>
```

### **10. View Commit History**
To see the commit history:
```sh
git log --oneline --graph --all
```

### **11. Revert Changes**
To discard unstaged changes:
```sh
git checkout -- <filename>
```
To reset staged changes:
```sh
git reset HEAD <filename>
```
To reset completely:
```sh
git reset --hard HEAD
```

### **12. Working with Remote Repositories**
To add a remote repository:
```sh
git remote add origin <repository-url>
```
To check remotes:
```sh
git remote -v
```

### **13. Handling Merge Conflicts**
If you get a merge conflict, Git will mark conflicting files. Open them, resolve conflicts manually, then:
```sh
git add <filename>
git commit -m "Resolved merge conflict"
```

### **14. Using Tags for Versioning**
To create a tag:
```sh
git tag -a v1.0 -m "Version 1.0 release"
```
To push tags:
```sh
git push origin --tags
```