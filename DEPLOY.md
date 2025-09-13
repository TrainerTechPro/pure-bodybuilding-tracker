# GitHub Deployment Guide

## Quick Deploy to GitHub Pages

Follow these simple steps to deploy your workout tracker to GitHub Pages for free:

### Step 1: Create GitHub Account
If you don't have one already, sign up at [github.com](https://github.com)

### Step 2: Create New Repository
1. Click the **"+"** button in the top right corner
2. Select **"New repository"**
3. Name it something like `workout-tracker` or `pure-bodybuilding-tracker`
4. Make it **Public** (required for free GitHub Pages)
5. Don't initialize with README (we already have one)
6. Click **"Create repository"**

### Step 3: Upload Files
1. Click **"uploading an existing file"** link
2. Drag and drop these files:
   - `workout-tracker.html` (rename to `index.html` before uploading)
   - `README.md`
   - `package.json`
3. Write a commit message like "Initial commit"
4. Click **"Commit changes"**

### Step 4: Enable GitHub Pages
1. Go to **Settings** tab in your repository
2. Scroll down to **"Pages"** section (in the left sidebar)
3. Under **"Source"**, select **"Deploy from a branch"**
4. Choose **"main"** branch and **"/ (root)"** folder
5. Click **"Save"**

### Step 5: Access Your Tracker
1. Wait 2-3 minutes for deployment
2. Your tracker will be available at:
   ```
   https://[your-username].github.io/[repository-name]
   ```
   Example: `https://johndoe.github.io/workout-tracker`

### Step 6: Bookmark on Your Phone
1. Open the URL on your phone's browser
2. Add to home screen for quick access
3. It will work like a native app!

## Updating Your Tracker

To make changes:
1. Edit the `index.html` file directly on GitHub
2. Or upload a new version
3. Changes will be live within minutes

## Custom Domain (Optional)

Want to use your own domain like `myworkouts.com`?
1. Buy a domain from any registrar
2. In repository Settings > Pages
3. Add your custom domain
4. Follow GitHub's DNS configuration guide

## Sharing with Friends

Your workout tracker is now public! Share the link with:
- Workout partners
- Personal trainers
- Anyone following the same program

## Privacy Note

While the app is publicly accessible, your personal workout data stays on YOUR device only. Each person using the link will have their own separate data stored locally.

## Troubleshooting

**Page not loading?**
- Wait a few more minutes after enabling Pages
- Check the Actions tab for deployment status
- Ensure file is named `index.html` not `workout-tracker.html`

**404 Error?**
- Double-check your URL
- Make sure GitHub Pages is enabled
- Repository must be public for free hosting

**Need Help?**
- Check GitHub Pages documentation
- Open an issue in the repository
- Contact GitHub support

---

## Alternative: Run Locally

If you prefer not to use GitHub:
1. Save `workout-tracker.html` to your computer
2. Double-click to open in browser
3. Bookmark the local file URL
4. Works offline forever!

Happy tracking! 💪