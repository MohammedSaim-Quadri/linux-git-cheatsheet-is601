# Linux + Git Cheat Sheet

This cheat sheet covers essential Linux and Git commands, with usage, flags, and examples.  

# Table of Contents
1. ls
2. cd
3. pwd
4. mkdir
5. touch
6. cp
7. mv
8. rm
9. cat
10. grep
11. chmod
12. git init
13. git clone
14. git config
15. git status
16. git add
17. git commit
18. git branch
19. git merge
20. git remote/ push / pull

---

## Linux Commands

### 1) ls
List files and directories.  
**Usage:** `ls -la`  
**Example:** `ls -lh /var/log`
**Flags:** `-a` show hidden, `-h` human-readable, `-l` long format

### 2) cd
Change directories.  
**Usage:** `cd /path/to/dir`  
**Examples:**
`cd ..` → go up one directory
`cd ~` → go to home

### 3) pwd
Print current working directory.  
**Usage:** `pwd`
**Note:** Useful when copying absolute paths.

### 4) mkdir
Create new directories.  
**Usage:** `mkdir -p project/src`
**Example:**`mkdir projects && cd projects`


### 5) touch
Create empty files / update timestamps.  
**Usage:** `touch notes.txt`
**Example:**`touch file1 file2 file3`; this creates multiple files at once

### 6) cp
Copy files and directories.  
**Usage:** `cp -r src dst`
**Example:**
Add interactive copy: `cp -i file.txt backup.txt`

### 7) mv
Move or rename files.  
**Usage:** `mv old.txt new.txt`

### 8) rm
Remove files or directories.  
**Usage:** `rm -rf mydir`

### 9) cat
Print file contents.  
**Usage:** `cat file.txt`

### 10) grep
Search inside files.  
**Usage:** `grep -i "error" logfile.log`

### 11) chmod
Change file permissions.  
**Usage:** `chmod +x script.sh`

---

## Git Commands

### 12) git init
Initialize a new Git repository in the current folder.  
**Usage:**  
```bash
git init
```

### 13) git clone
Clone (download) a repo from GitHub.
***Usage:***
```bash
git clone git@github.com:user/repo.git
```

### 14) git config
Configure user information for commits.
***Usage:***
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

### 15) git status
Show repo status (modified, staged, untracked files).
***Usage:***
```bash
git status
```

### 16) git add
Stage changes for commit.
***Usage:***
```bash
git add file.txt or git add .
```

### 17) git commit
Save changes to history.
***Usage:***
```bash
git commit -m "Message"
```

### 18) git branch
List or create branches.
***Usage:***
```bash
git branch         # list
git branch feature # create
```

### 19) git merge
Merge one branch into another.
***Usage:***
```bash
git switch main
git merge feature
```

### 20) git remote / push / pull
Connect with remotes and sync.
***Usage:***
```bash
git remote add origin git@github.com:user/repo.git
git push -u origin main
git pull
```
