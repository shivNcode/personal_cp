To make GitHub upload **only your `.cpp` files** and ignore everything else, you just need to configure a **`.gitignore`** file correctly.

## ✅ **Step-by-step: Make Git ignore all files except `.cpp`**

### **1️⃣ Create a `.gitignore` file in your project folder**

Inside your project folder (VS Code), create a file named:

```
.gitignore
```

### **2️⃣ Add this content:**

```
# Ignore everything
*

# But NOT these:
!*.cpp
!.gitignore
```

### ✔ Explanation:

- `*` → ignore all files
    
- `!*.cpp` → do NOT ignore `.cpp` files
    
- `!.gitignore` → keep the ignore file itself
    

So only your `.cpp` files will be pushed to GitHub.

---

## ⭐ If your `.cpp` files are inside folders

Git will also ignore folders unless you explicitly allow them.

Use this better version:

```
# Ignore everything
*

# Allow folders
!*/

# Allow C++ files
!*.cpp

# Keep this file
!.gitignore
```

---

## 🚀 Now upload to GitHub

Run these commands:

```bash
git add .
git commit -m "Upload only cpp files"
git push origin main
```

---

