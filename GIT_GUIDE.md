# 🔧 Git Quick Reference Guide

Copy and paste these commands when working with your GitHub repository.

## Initial Setup (First Time Only)

```bash
# Navigate to your project folder
cd "c:\Users\DONEX\Documents\my codes\SOLAR ENERGY"

# Initialize Git
git init

# Configure Git (one-time)
git config user.name "Your Name"
git config user.email "your.email@example.com"

# Add all files
git add .

# First commit
git commit -m "Initial commit: Solar calculator application"

# Add remote (replace with your actual repo URL)
git remote add origin https://github.com/yourusername/engineerdogo-solar-calculator.git

# Rename branch to main
git branch -M main

# Push to GitHub
git push -u origin main
```

## Regular Workflow (After Setup)

### Save Changes Locally
```bash
# See what changed
git status

# Add specific file
git add filename.html

# Or add all changes
git add .

# Create a checkpoint (commit)
git commit -m "Brief description of what changed"
```

### Push to GitHub
```bash
# Send to GitHub
git push

# Or if it's a new branch
git push -u origin main
```

### Complete Save & Push (Quick)
```bash
# Do this after making changes
git add .
git commit -m "What changed"
git push
```

## Checking Status

```bash
# See current status
git status

# See what files changed
git diff

# See commit history
git log

# See remote info
git remote -v
```

## Common Scenarios

### "I want to undo my last commit"
```bash
# Keep changes locally, undo commit
git reset --soft HEAD~1

# Discard changes completely
git reset --hard HEAD~1
```

### "I want to see what I changed"
```bash
# Show specific file changes
git diff filename.html

# Show all changes
git diff
```

### "I forgot to add a file to my last commit"
```bash
# Add the file
git add forgotten-file.html

# Amend the last commit
git commit --amend --no-edit
```

### "I want to create a new branch for testing"
```bash
# Create and switch to new branch
git checkout -b feature/new-feature

# Do your work...

# Push new branch
git push -u origin feature/new-feature
```

### "I want to go back to a previous version"
```bash
# See all commits
git log

# Copy the commit ID (hash)
# Check out that version
git checkout <commit-hash>

# Go back to latest
git checkout main
```

## Useful Aliases (Optional)

Add these to your Git config to save typing:

```bash
# Add some aliases
git config --global alias.st status
git config --global alias.co checkout
git config --global alias.cm commit
git config --global alias.ps push
git config --global alias.pl pull

# Then you can use:
git st          # instead of git status
git cm -m "msg" # instead of git commit -m "msg"
git ps          # instead of git push
```

## Essential Commands Reference

| Command | What It Does | Example |
|---------|-------------|---------|
| `git init` | Start Git in folder | `git init` |
| `git add` | Stage files for commit | `git add index.html` |
| `git commit` | Save staged changes | `git commit -m "Fix button"` |
| `git push` | Send to GitHub | `git push` |
| `git pull` | Get latest from GitHub | `git pull` |
| `git status` | See what changed | `git status` |
| `git log` | See commit history | `git log` |
| `git diff` | See specific changes | `git diff file.html` |
| `git clone` | Copy repo from GitHub | `git clone https://...` |
| `git branch` | List/create branches | `git branch new-branch` |
| `git checkout` | Switch branch/version | `git checkout main` |

## 🚨 Important Notes

### Before You Push
1. Always `git status` to see what you're pushing
2. Commit messages should describe changes clearly
3. Don't commit passwords or API keys
4. Keep commits small and focused

### Good Commit Messages
```bash
# ✅ GOOD
git commit -m "Fix PDF export filename"
git commit -m "Add cable sizing for DC circuits"
git commit -m "Update color scheme to cyan/orange"

# ❌ BAD
git commit -m "fix"
git commit -m "stuff"
git commit -m "asdlkf"
```

### If Something Goes Wrong
```bash
# See what happened
git log

# Reset to a safe point
git reset --hard <commit-hash>

# Still confused? Don't push, ask for help first!
```

## Connection Issues

### "Permission denied (publickey)"
```bash
# Set up SSH key (recommended)
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

# Or switch to HTTPS
git remote set-url origin https://github.com/yourusername/repo.git
```

### "fatal: not a git repository"
```bash
# Make sure you're in the right folder
cd "c:\Users\DONEX\Documents\my codes\SOLAR ENERGY"

# Initialize if needed
git init
```

## Windows-Specific Notes

### Using Command Prompt/PowerShell
- All commands work the same
- Use backslashes for paths: `cd C:\path\to\folder`
- Or use forward slashes: `cd C:/path/to/folder`

### Using Git Bash (Recommended)
- Follows Unix conventions
- Better experience on Windows
- Download from: https://git-scm.com

## Advanced Tips

### Viewing differences with a tool
```bash
# Use visual diff tool
git difftool filename.html
```

### Creating backups before major changes
```bash
# Create a backup branch
git branch backup-$(date +%Y%m%d)
git push -u origin backup-$(date +%Y%m%d)
```

### Tracking file size
```bash
# See which files are largest
git ls-files -s | sort -k4 -rn | head -20
```

---

## 📚 More Help

- GitHub docs: https://docs.github.com/en/get-started/using-git
- Git docs: https://git-scm.com/doc
- Markdown syntax: https://www.markdownguide.org
- Emoji cheatsheet: https://github.com/ikatyang/emoji-cheat-sheet

---

**Copy these commands as you need them. You've got this! 💪⚡**
