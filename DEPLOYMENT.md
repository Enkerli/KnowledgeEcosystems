# Deployment Guide

This guide explains how to push this project to GitHub and deploy it on GitHub Pages.

## Prerequisites

- A GitHub account
- Git configured with your GitHub credentials
- Command line access

## Step 1: Create a New GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right and select "New repository"
3. Configure the repository:
   - **Repository name**: `KnowledgeEcosystems` (or your preferred name)
   - **Description**: "Interactive visualization of parallel timelines of disciplines, institutions, and knowledge regimes from 20,000 BCE to present"
   - **Visibility**: Public
   - **Do NOT initialize** with README, .gitignore, or license (we already have these)
4. Click "Create repository"

## Step 2: Push Local Repository to GitHub

After creating the repository, GitHub will show you instructions. Use these commands:

```bash
# Add the GitHub remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/KnowledgeEcosystems.git

# Push the code to GitHub
git branch -M main
git push -u origin main
```

If you prefer SSH (recommended for frequent commits):

```bash
git remote add origin git@github.com:YOUR_USERNAME/KnowledgeEcosystems.git
git branch -M main
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" (gear icon)
3. Scroll down to "Pages" in the left sidebar
4. Under "Source":
   - Select branch: **main**
   - Select folder: **/ (root)**
5. Click "Save"

GitHub will now deploy your site. The URL will be:
```
https://YOUR_USERNAME.github.io/KnowledgeEcosystems/
```

It may take a few minutes for the first deployment.

## Step 4: Update README with Live Links

Once deployed, update the README.md with your actual URLs:

```bash
# Edit README.md and replace placeholder links with:
# - Live Demo: https://YOUR_USERNAME.github.io/KnowledgeEcosystems/
# - Repository: https://github.com/YOUR_USERNAME/KnowledgeEcosystems
# - Issues: https://github.com/YOUR_USERNAME/KnowledgeEcosystems/issues
# - Discussions: https://github.com/YOUR_USERNAME/KnowledgeEcosystems/discussions

# Commit the changes
git add README.md
git commit -m "Update README with live deployment links"
git push
```

## Step 5: Verify Deployment

1. Visit your GitHub Pages URL
2. Test the interactive visualization:
   - Timeline should render correctly
   - All 487 entries should load
   - Filters and storyline chips should work
   - Clicking entries should show details
3. Check that all links work

## Optional: Custom Domain

If you have a custom domain:

1. In repository Settings → Pages
2. Under "Custom domain", enter your domain
3. Add DNS records as instructed by GitHub
4. Enable "Enforce HTTPS" (recommended)

## Troubleshooting

### Site not loading

- Wait a few minutes after enabling Pages (first deployment takes time)
- Check Settings → Pages for deployment status
- Look for errors in the "Actions" tab

### Data not loading

- Check browser console for errors (F12 → Console tab)
- Verify `data.json` was committed and pushed
- Ensure file permissions are correct (should be readable)

### Visualization not rendering

- Check that `index.html` references `data.json` with relative path `./data.json`
- Clear browser cache and reload (Ctrl+Shift+R or Cmd+Shift+R)
- Test in different browsers

## Future Updates

To update the deployed site:

```bash
# Make changes to files
# ...

# Commit changes
git add .
git commit -m "Description of changes"

# Push to GitHub (will auto-deploy)
git push
```

GitHub Pages will automatically rebuild and redeploy within a few minutes.

## Sharing Your Work

Once deployed, share your visualization:

- Tweet the link with #DataViz #HistoryOfScience
- Post on relevant subreddits (r/dataisbeautiful, r/HistoryOfScience)
- Share in academic networks and digital humanities communities
- Add to your CV/portfolio

## Repository Settings Recommendations

### Enable Discussions
Settings → General → Features → Check "Discussions"

This allows community engagement and questions.

### Add Topics
Repository → About (gear icon) → Add topics:
- `data-visualization`
- `history-of-science`
- `knowledge-systems`
- `digital-humanities`
- `interactive-timeline`
- `public-domain`

### Set Social Preview
Repository → Settings → General → Social preview
Upload a screenshot of the visualization (1280x640px recommended)

### Enable Issues
Should be enabled by default. Use for:
- Bug reports
- Feature requests
- Dataset corrections
- New entry suggestions

## License Reminder

This project is released under CC0 1.0 Universal (Public Domain Dedication).
Anyone can use, modify, and distribute it freely without attribution requirements.

Consider adding a CC0 badge to your repository:
Settings → General → About → Edit → Select CC0-1.0 in "License"

---

**Ready to Deploy!**

Your knowledge ecosystems visualization is ready to share with the world.
