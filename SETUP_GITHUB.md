# 🚀 GitHub Setup & Hosting Guide

This guide will walk you through publishing the EngineerDogo Solar System Calculator on GitHub Pages so anyone can access it online.

## Prerequisites

- GitHub account (free at [github.com](https://github.com))
- Git installed on your computer ([git-scm.com](https://git-scm.com))
- Basic command line knowledge (minimal)

## 📋 Step-by-Step Setup

### Step 1: Create a New GitHub Repository

1. Go to [github.com](https://github.com) and log in
2. Click the **"+"** icon in the top-right corner
3. Select **"New repository"**
4. Fill in the details:
   - **Repository name**: `engineerdogo-solar-calculator` (can be any name)
   - **Description**: "Advanced Solar System Calculator for inverter, battery, and panel sizing"
   - **Public**: Make sure it's set to **Public** (required for GitHub Pages)
   - **Initialize with README**: No (we already have one)
5. Click **"Create repository"**

### Step 2: Prepare Your Local Folder

1. Open Command Prompt or Terminal
2. Navigate to your project folder:
   ```bash
   cd "c:\Users\DONEX\Documents\my codes\SOLAR ENERGY"
   ```

3. Initialize Git in this folder:
   ```bash
   git init
   ```

4. Add all files:
   ```bash
   git add .
   ```

5. Create your first commit:
   ```bash
   git commit -m "Initial commit: EngineerDogo Solar Calculator"
   ```

### Step 3: Connect to GitHub & Push Code

1. Go back to your new GitHub repository page
2. Copy the repository URL (HTTPS):
   ```
   https://github.com/yourusername/engineerdogo-solar-calculator.git
   ```

3. In your command line, add the remote:
   ```bash
   git remote add origin https://github.com/yourusername/engineerdogo-solar-calculator.git
   ```

4. Rename your branch (if needed):
   ```bash
   git branch -M main
   ```

5. Push your code:
   ```bash
   git push -u origin main
   ```

   (You may be prompted for your GitHub username and password)

### Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (in the top right)
3. In the left sidebar, click **Pages**
4. Under **Build and deployment**:
   - **Source**: Select `Deploy from a branch`
   - **Branch**: Select `main` (or `master`)
   - **Folder**: Select `/ (root)`
5. Click **Save**

5. Wait 1-2 minutes for GitHub to build your site
6. You'll see a message with your live URL:
   ```
   ✅ Your site is live at: https://yourusername.github.io/engineerdogo-solar-calculator/
   ```

## 🌐 Accessing Your Site

After GitHub Pages finishes building:

- **Project Page**: `https://yourusername.github.io/engineerdogo-solar-calculator/`
- **Direct File**: `https://yourusername.github.io/engineerdogo-solar-calculator/index.html`

Share this URL with anyone to let them use your calculator!

## 📁 File Structure

Your GitHub repository should have these files:

```
engineerdogo-solar-calculator/
├── index.html                 ← Main application (GitHub Pages will serve this)
├── EngineerDogo.html          ← Alternative copy
├── README.md                  ← Project documentation
├── LICENSE                    ← MIT License
├── .gitignore                 ← What to ignore in Git
└── SETUP_GITHUB.md           ← This file
```

## 🔄 Making Updates

After your initial setup, whenever you want to update the site:

1. Make changes to your files locally
2. In command line:
   ```bash
   git add .
   git commit -m "Your change description here"
   git push
   ```
3. GitHub will automatically rebuild your site (usually within 1-2 minutes)

## 🆘 Troubleshooting

### "Site is not published yet"
- Wait 2-3 minutes after enabling Pages
- Refresh the page
- Check that `index.html` exists in the root folder
- Ensure repository is **Public**

### "404 - Page Not Found"
- Verify the URL matches your repository name
- Make sure `index.html` is in the root directory
- Check browser console (F12) for errors

### "Push rejected"
- Ensure you're in the correct folder
- Verify remote is set correctly: `git remote -v`
- Check GitHub credentials are saved

## 📊 Checking Build Status

1. Go to your repository on GitHub
2. Click the **"Deployments"** tab
3. Look for "github-pages" deployment
4. Check the status (✓ Active, ⏳ In progress, ✗ Failed)

## 🔐 Advanced: Custom Domain (Optional)

If you have a custom domain (e.g., yourname.com):

1. In GitHub repository Settings → Pages
2. Under "Custom domain", enter your domain
3. Update your domain's DNS settings (see provider instructions)
4. GitHub will automatically set up HTTPS

## 📚 Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Git Basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)
- [Markdown Guide](https://www.markdownguide.org/)

## 🎉 Congratulations!

Your EngineerDogo Solar System Calculator is now live on the internet! 

Share the link with:
- 👨‍🔧 Engineers and technicians
- ☀️ Solar installers
- 🏠 Homeowners planning solar systems
- 🌍 Anyone interested in off-grid power

---

**Having issues?** Check the [GitHub Help Documentation](https://docs.github.com/en) or open an issue in your repository!
