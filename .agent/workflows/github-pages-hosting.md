---
description: How to host the Silent Byte website on GitHub Pages for free
---

# Hosting on GitHub Pages

Follow these steps to deploy your Silent Byte website to GitHub Pages for free hosting.

## Prerequisites
- Git installed on your computer
- GitHub account (create at https://github.com if needed)

## Step 1: Initialize Git Repository (if not done)

Open PowerShell/Terminal in your project folder:

```powershell
cd "e:\Silent_byte\Silent_Byte"
git init
git add .
git commit -m "Initial commit - Silent Byte website"
```

## Step 2: Create GitHub Repository

1. Go to https://github.com/new
2. Repository name: `Silent_Byte` (or any name you prefer)
3. Set to **Public** (required for free GitHub Pages)
4. Do NOT initialize with README (you already have files)
5. Click **Create repository**

## Step 3: Push to GitHub

After creating the repo, GitHub will show you commands. Run these:

```powershell
git remote add origin https://github.com/YOUR_USERNAME/Silent_Byte.git
git branch -M main
git push -u origin main
```

Replace `YOUR_USERNAME` with your actual GitHub username.

## Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Scroll down to **Pages** (left sidebar)
4. Under "Source", select **Deploy from a branch**
5. Choose **main** branch and **/ (root)** folder
6. Click **Save**

## Step 5: Access Your Website

After a few minutes, your site will be live at:

```
https://YOUR_USERNAME.github.io/Silent_Byte/
```

## Updating Your Website

Whenever you make changes, push them to GitHub:

```powershell
git add .
git commit -m "Description of changes"
git push
```

GitHub Pages will automatically redeploy within a few minutes.

## Custom Domain (Optional)

To use your own domain:
1. Go to Settings > Pages
2. Under "Custom domain", enter your domain
3. Add a CNAME record pointing to `YOUR_USERNAME.github.io`
4. Create a file called `CNAME` in your repo with your domain name

---

> **Tip**: GitHub Pages is completely free for public repositories!
