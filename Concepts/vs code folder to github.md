
---

# 📘 Documentation: Uploading a VS Code Folder to GitHub Repository

## 📌 Purpose

This document explains how to upload an existing **local folder opened in VS Code** to **GitHub** by creating a new repository and pushing code using **Git**.

---

## 🛠 Prerequisites

Make sure the following are installed and ready:

- **Git** installed (`git --version` to check)
    
- **VS Code**
    
- **GitHub account**
    
- Folder already opened in **VS Code**
    

---

## 📂 Step 1: Open Terminal in VS Code

1. Open your project folder in VS Code
    
2. Open terminal using:
    
    - `Ctrl +` (Windows/Linux)
        
    - `Cmd +` (Mac)
        
3. Ensure terminal path points to your project directory
    

---

## 🧩 Step 2: Initialize Git Repository

Run the following command:

```bash
git init
```

### ✅ Result

- A hidden `.git` folder is created
    
- Your folder becomes a Git repository
    

---

## 📊 Step 3: Check Repository Status (Optional)

```bash
git status
```

### Output:

- Files will appear as **untracked**
    

---

## ➕ Step 4: Add Files to Staging Area

Add all files:

```bash
git add .
```

### What this does:

- Prepares files for commit
    
- Moves files to staging area
    

---

## 📝 Step 5: Commit Changes

Create the first commit:

```bash
git commit -m "Initial commit"
```

### Meaning:

- Saves a snapshot of your project
    
- `"Initial commit"` is the commit message
    

---

## 🌐 Step 6: Create Repository on GitHub

1. Go to **github.com**
    
2. Click **+ → New repository**
    
3. Enter:
    
    - Repository Name
        
    - Visibility (Public / Private)
        
4. ❌ Do **NOT** select:
    
    - Add README
        
    - Add .gitignore
        
    - Choose a license
        
5. Click **Create repository**
    

---

## 🔗 Step 7: Link Local Repo to GitHub Repo

Run the commands shown on GitHub:

```bash
git branch -M main
git remote add origin https://github.com/USERNAME/REPO_NAME.git
```

📌 Replace:

- `USERNAME` → your GitHub username
    
- `REPO_NAME` → repository name
    

---

## 🚀 Step 8: Push Code to GitHub

```bash
git push -u origin main
```

### Authentication:

- Username → GitHub username
    
- Password → **GitHub Personal Access Token (PAT)**
    

---

## ✅ Final Result

- Your local folder is now uploaded to GitHub
    
- Repository contains all project files
    
- `main` branch is set as default
    

---

## ⚠️ Common Errors & Solutions

### ❌ Error: `remote origin already exists`

**Fix:**

```bash
git remote remove origin
git remote add origin <repo-url>
```

---

### ❌ Error: `failed to push some refs`

**Fix:**

```bash
git pull origin main --rebase
git push origin main
```

---

### ❌ Authentication Failed

**Reason:** GitHub no longer accepts passwords  
**Fix:** Use **Personal Access Token (PAT)**

---

## 💡 Alternative: VS Code UI Method

1. Click **Source Control (Git icon)**
    
2. Click **Initialize Repository**
    
3. Stage files → Commit
    
4. Click **Publish to GitHub**
    

---

## 📦 Next Steps (After Upload)

- Make changes → `git add .`
    
- Commit → `git commit -m "message"`
    
- Push → `git push`
    

---

## 📌 Best Practices

- Add `.gitignore` (node_modules, build, .env, etc.)
    
- Write meaningful commit messages
    
- Push frequently
    
- Keep repository clean
    

---

