
<img width="1536" height="1024" alt="first-project" src="https://github.com/user-attachments/assets/fd9b6d79-3717-4fa4-b2cc-224b7f3aa5e6" />

# 🐍 **Easy-to-Use Python Project Setup: Connect GitHub to Your Local**

**⚡ Future-proof & ready for packaging, perfect for beginners**

Getting from *writing code* to *managing a professional project* can feel overwhelming. This guide walks you through creating a **Python project** that’s **structured, maintainable, and connected to GitHub**—step by step.

We’ll use **`uv`** to set up your project professionally from day one.

---

## 📌 **First, Some Preliminaries**

Before we start, here’s what you need to know:

* **Why `uv`?**

  * ✅ Creates a **clean project structure** (`src/` layout)
  * ✅ Locks dependencies for **consistent behavior** across computers
  * ✅ Makes **future packaging and sharing** easy

* **Why not `pip`?**

  * ❌ No lockfile by default
  * ❌ No enforced project structure
  * ❌ Less predictable dependency management

* **Prerequisites:**

  * **Git**: Version control system to connect your project to GitHub. [Download Git](https://git-scm.com)
  * **uv**: Python project management tool. [Download uv](https://uv.org)

> ✅ **Once Git and `uv` are installed, you’re ready to start.**

---

## Step 1: **Create Your GitHub Repository**

**Goal:** Set up your remote **“Source of Truth.”**

1. Go to [GitHub.com](https://github.com) and sign up if you don’t have an account.
2. Click the **green [New] button**.
3. **Name your repository:** `first-repo`
4. **Set visibility:**

   * 🔒 **Private:** Only you and invited collaborators can see it
   * 🌍 **Public:** Anyone can view it
5. ⚠️ **Important:** Do **not** check “Add a README” or “.gitignore.”

   > The repository must be **empty** for the Handshake to work smoothly.
6. Click **Create repository** ✅

> Your empty GitHub repository is ready!

---

## Step 2: **Prepare Your Local Workspace**

**Goal:** Create a clean folder for your project on your computer.

```bash
mkdir first-repo   # Create the project folder
cd first-repo      # Move into the folder
rm -rf .git        # Remove any existing Git configuration
```

> ✅ Local workspace is ready.

---

## Step 3: **Configure Your Project**

**Goal:** Initialize your project with a professional layout and lock dependencies.

```bash
uv init --lib       # Creates src/ folder and project structure
uv sync             # Generates uv.lock for dependencies
```

> ✅ Your project now has a professional **src/ layout** and locked dependencies.

---

## Step 4: **Connect Your Project to GitHub**

**Goal:** Link your local project to your remote repository and push your first commit.

```bash
git init
git add .
git commit -m "initial setup"
git branch -M main
git remote add origin https://github.com/USER/first-repo.git
git push -u origin main
```

> Replace `USER` with your GitHub username.

> ✅ Your project is now connected to GitHub! Future changes can be committed and pushed.

---

## ✅ **Next Steps**

* 💻 Start coding in `src/first_repo/`
* 🧪 Add tests in `tests/` and run them with `pytest`
* 🔄 Commit changes regularly and push to GitHub
* 📦 Explore publishing your project as a Python package later

