# Web Playground - Git Workflow Guide

## Initial Setup

```bash
# Configure Git (first time only)
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
git config --global init.defaultBranch main

# Initialize repository
git init
git add .
git commit -m "feat: initial commit"

# Stage files
git add filename          # Specific file
git add .              # All changes

# Commit with meaningful message
git commit -m "feat: add user authentication"
git commit -m "fix: resolve header alignment issue"

#Handling Merge conflicts
# Stash your local changes
git stash

# Pull latest changes
git pull origin main

# Apply your stashed changes back
git stash pop

# Resolve any conflicts manually, then:
git add .
git commit -m "fix: merge conflicts resolved"