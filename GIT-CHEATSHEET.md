
# 🧾 Git + GitHub Cheatsheet (Karen Edition)

## 📁 SETUP: First Time You’re Connecting a Local Project to GitHub

```bash
# Step 1: In your project folder
git init

# Step 2: Add and commit your code
git add .
git commit -m "Initial commit"

# Step 3: Link to GitHub repo
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# Step 4: Set your branch to 'main' and push
git branch -M main
git push -u origin main
```

> ✅ After this, you can just do `git push` every time. You're linked.

---

## 🔁 EVERYDAY WORKFLOW

```bash
# 1. See what changed
git status

# 2. Stage your changes
git add .

# 3. Commit with a message
git commit -m "Add new feature / fix bug / update styles"

# 4. Push it to GitHub
git push
```

---

## 🔄 IF YOUR GITHUB REPO HAS A README (OR ANY FILE)

```bash
# You'll likely need to pull before first push
git pull origin main --allow-unrelated-histories
git push -u origin main
```

---

## 🧭 CHECKING CONFIGS

```bash
# Who am I as far as Git is concerned?
git config --global user.name
git config --global user.email

# Who am I pushing to?
git remote -v
```

---

## 🧹 OTHER GOODIES

```bash
# Rename the current branch to main (in case it's still called master)
git branch -M main

# Undo a file you staged (before commit)
git reset <file>

# See all commits
git log

# Clone someone else's repo (or your own)
git clone https://github.com/username/repo-name.git
```

---

## 🧠 PRO TIP: Writing Good Commits

Try using small, clear commits with active language:

```bash
git commit -m "Add click counter component"
git commit -m "Fix styling bug in RedButton"
git commit -m "Update README with setup instructions"
```
