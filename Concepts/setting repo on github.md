
---

# ✅ **One-Time Setup (Do this once)**

## **1. Copy your GitHub repo URL**

Go to your repo → click **Code → HTTPS → copy the link**  
Example:

```
https://github.com/your-username/your-repo.git
```

## **2. Clone the repo in your laptop**

Open VS Code → open terminal → run:

```bash
git clone https://github.com/your-username/your-repo.git
```

Now your repo folder is on your local machine.

## **3. Open that folder in VS Code**

```
File → Open Folder → select your repo folder
```

---

# ✅ **Daily Workflow (Use this EVERY DAY)**

Whenever you make changes and want to update GitHub:

---

## **1. Check which files changed**

In VS Code terminal:

```bash
git status
```

---

## **2. Add all updated files**

```bash
git add .
```

---

## **3. Commit with a message**

Give a message describing today’s change:

```bash
git commit -m "Updated files for today"
```

---

## **4. Push to GitHub**

Send updates to GitHub:

```bash
git push origin main
```

⚠️ _If your branch name is `master` instead of `main`:_

```bash
git push origin master
```

---

# 🎯 **Your Daily Routine (Short Version)**

Run these 3 commands everyday after editing:

```bash
git add .
git commit -m "update"
git push
```

That's it — your repo will be updated on GitHub.

---

# 📝 Optional Good Practice

If you're working from multiple devices or if your repo gets updates:

```bash
git pull
```

This pulls the latest changes from GitHub before you start work.

---
