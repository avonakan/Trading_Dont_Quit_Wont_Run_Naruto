# GitHub Repository Setup Guide

## Step 1: Create a Private GitHub Repository

1. **Go to GitHub:**
   - Visit https://github.com
   - Log in to your account

2. **Create New Repository:**
   - Click the `+` icon in the top-right corner
   - Select `New repository`

3. **Configure Repository:**
   - **Repository name:** `stock-analysis` (or your preferred name)
   - **Description:** "Stock trading analysis tool using moving averages"
   - **Privacy:** Select `Private` ⚠️ IMPORTANT
   - **Initialize:** 
     - ❌ Do NOT check "Add a README file"
     - ❌ Do NOT add .gitignore yet
     - ❌ Do NOT add license yet
   - Click `Create repository`

## Step 2: Set Up Local Repository

Open your terminal/command prompt and run:

```bash
# Create a new directory for your project
mkdir stock-analysis
cd stock-analysis

# Initialize git repository
git init

# Add your files to the directory
# (Copy all the files from the outputs: Stock_Analysis_Updated.ipynb, README.md, etc.)

# Add all files to git
git add .

# Commit the files
git commit -m "Initial commit: Stock analysis notebook with buy/sell analysis"

# Add your GitHub repository as remote
# Replace YOUR_USERNAME with your GitHub username
git remote add origin https://github.com/YOUR_USERNAME/stock-analysis.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 3: Using with Google Colab

### Method 1: Direct Upload (Easiest)

1. Go to [Google Colab](https://colab.research.google.com/)
2. Click `File` → `Upload notebook`
3. Upload your `Stock_Analysis_Updated.ipynb`
4. Use normally

### Method 2: Connect to GitHub (Best Practice)

1. **Mount GitHub in Colab:**
   ```python
   # In a Colab cell, run:
   from google.colab import drive
   drive.mount('/content/drive')
   ```

2. **Clone your repository:**
   ```python
   !git clone https://github.com/YOUR_USERNAME/stock-analysis.git
   %cd stock-analysis
   ```

3. **Open the notebook:**
   - In Colab, navigate to `File` → `Open notebook` → `GitHub` tab
   - Enter your repository URL: `https://github.com/YOUR_USERNAME/stock-analysis`
   - Select `Stock_Analysis_Updated.ipynb`

4. **Make it easier with GitHub integration:**
   - Colab → `File` → `Save a copy in GitHub`
   - This will save changes directly to your repo

## Step 4: Best Practices for Version Control

### Regular Workflow

```bash
# Before making changes, pull latest version
git pull origin main

# Make your changes to the notebook or code
# ...

# Check what changed
git status

# Add changes
git add Stock_Analysis_Updated.ipynb
# Or add all changes
git add .

# Commit with meaningful message
git commit -m "Added new feature: sector analysis"

# Push to GitHub
git push origin main
```

### Useful Git Commands

```bash
# View commit history
git log --oneline

# Create a new branch for experiments
git checkout -b feature/new-analysis

# Switch back to main branch
git checkout main

# Merge feature branch into main
git merge feature/new-analysis

# View remote repository URL
git remote -v

# Discard local changes
git checkout -- Stock_Analysis_Updated.ipynb
```

## Step 5: Security Checklist

✅ Repository is set to **Private**
✅ `.gitignore` includes all sensitive file patterns (*.csv, *.xlsx)
✅ Never commit files with actual trading data
✅ Use environment variables for any API keys (if added later)
✅ Review files before committing: `git status` and `git diff`

## Step 6: Sharing Access (Optional)

If you want to share with collaborators:

1. Go to your repository on GitHub
2. Click `Settings` → `Collaborators`
3. Click `Add people`
4. Enter their GitHub username or email
5. They'll receive an invitation

## Step 7: Backing Up from Colab

To save your Colab work to GitHub automatically:

1. In Colab: `File` → `Save a copy in GitHub`
2. Select your repository
3. Choose the branch (usually `main`)
4. Add a commit message
5. Click `OK`

## Troubleshooting

### Authentication Issues

If GitHub asks for credentials:

```bash
# Use Personal Access Token instead of password
# Generate at: GitHub → Settings → Developer settings → Personal access tokens
# Select scopes: repo (all)

# Configure Git to use token
git remote set-url origin https://YOUR_USERNAME:YOUR_TOKEN@github.com/YOUR_USERNAME/stock-analysis.git
```

### Large File Warning

If you accidentally committed large files:

```bash
# Remove file from Git but keep locally
git rm --cached filename.csv

# Add to .gitignore
echo "filename.csv" >> .gitignore

# Commit the changes
git add .gitignore
git commit -m "Remove sensitive data and update .gitignore"
git push origin main
```

## Additional Tips

1. **Create a backup branch before major changes:**
   ```bash
   git checkout -b backup-$(date +%Y%m%d)
   git push origin backup-$(date +%Y%m%d)
   ```

2. **Tag important versions:**
   ```bash
   git tag -a v1.0 -m "Initial working version"
   git push origin v1.0
   ```

3. **Keep a CHANGELOG.md** to track major updates

4. **Use GitHub Issues** to track TODOs and bugs

5. **Enable GitHub Actions** for automated testing (advanced)

---

## Quick Reference Card

```bash
# Daily workflow
git pull                          # Get latest changes
# ... make changes ...
git add .                         # Stage all changes
git commit -m "Description"       # Commit changes
git push origin main              # Push to GitHub

# Check status
git status                        # What's changed?
git diff                          # Show exact changes
git log --oneline -5             # Last 5 commits

# Undo changes
git checkout -- filename          # Discard local changes
git reset HEAD filename           # Unstage file
git revert <commit-hash>         # Undo a commit
```

---

**You're all set! Happy coding! 🚀**
