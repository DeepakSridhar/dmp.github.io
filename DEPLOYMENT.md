# Deployment Guide

## Quick Start Checklist

- [ ] Add `DMP_NeurIPS_2026.pdf` to the root directory
- [ ] Extract figures from PDF (see `images/README.md`)
- [ ] Test website locally by opening `index.html` in a browser
- [ ] Update GitHub repository name if needed
- [ ] Push to GitHub
- [ ] Enable GitHub Pages
- [ ] Visit your live site!

## Detailed Steps

### 1. Add Required Files

```bash
# Make sure you're in the project directory
cd d:/PhD/Website/dmp.github.io

# Add your PDF file (copy it to this directory)
# Then verify it's here:
ls -la DMP_NeurIPS_2026.pdf
```

### 2. Extract and Add Images

Follow the guide in `images/README.md` to extract the following images from your PDF:

Required images (8 total):
- `teaser.png` - Main comparison figure
- `method.png` - DMP framework diagram
- `composite_results.png` - Classification results table
- `hierarchical_results.png` - Bar chart
- `variation_results.png` - Variation synthesis results
- `composition.png` - Identity composition examples
- `negative_prompting.png` - Negative prompting examples
- `generalization.png` - Generalization comparison

### 3. Test Locally

Open `index.html` in your web browser:

**Windows:**
```bash
start index.html
```

**Mac:**
```bash
open index.html
```

**Linux:**
```bash
xdg-open index.html
```

Check that:
- All sections display correctly
- Images load properly (no broken image icons)
- Links work
- Page is responsive (resize browser window)

### 4. Initialize Git Repository (if not done)

```bash
cd d:/PhD/Website/dmp.github.io

# Initialize git (already done in your case)
# git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: DMP project website"
```

### 5. Create GitHub Repository

**Option A: Via GitHub Website**
1. Go to https://github.com/new
2. Repository name: `dmp.github.io` (or your preferred name)
3. Description: "Project page for Diffusion Meta-Prompting (NeurIPS 2026)"
4. Choose Public
5. Don't initialize with README (you already have one)
6. Click "Create repository"

**Option B: Via GitHub CLI**
```bash
gh repo create dmp.github.io --public --source=. --remote=origin
```

### 6. Push to GitHub

```bash
# Add remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/dmp.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### 7. Enable GitHub Pages

**Method 1: Via GitHub Website**
1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" section (left sidebar)
4. Under "Source", select "main" branch
5. Keep the folder as "/ (root)"
6. Click "Save"
7. Wait a few minutes, your site will be live at:
   `https://YOUR_USERNAME.github.io/dmp.github.io/`

**Method 2: Via GitHub CLI**
```bash
gh repo edit --enable-pages --pages-branch main
```

### 8. Update Links (Optional)

Once your site is live, you may want to update the README with the actual URL:

1. Open `README.md`
2. Replace `[your-username]` with your actual GitHub username
3. Commit and push:
   ```bash
   git add README.md
   git commit -m "Update README with live site URL"
   git push
   ```

### 9. Verify Deployment

After a few minutes, visit your site:
- `https://YOUR_USERNAME.github.io/dmp.github.io/`

If it doesn't work immediately:
- Wait 5-10 minutes (GitHub Pages can take time to build)
- Check the "Actions" tab in your repository for build status
- Verify GitHub Pages is enabled in Settings

## Updating the Website

After making changes:

```bash
# After editing files locally
git add .
git commit -m "Description of changes"
git push

# GitHub Pages will automatically rebuild (takes 1-2 minutes)
```

## Troubleshooting

### Images not showing
- Check that image files are in the `images/` folder
- Verify filenames match exactly (case-sensitive)
- Ensure images are committed and pushed to GitHub

### CSS not loading
- Clear browser cache (Ctrl+F5 or Cmd+Shift+R)
- Check that `style.css` is in the same directory as `index.html`
- Verify the file was pushed to GitHub

### 404 Error
- Make sure GitHub Pages is enabled
- Check that you're using the correct URL
- Wait a few more minutes for build to complete

### PDF not downloadable
- Ensure `DMP_NeurIPS_2026.pdf` is in the root directory
- Check it's pushed to GitHub
- Verify the link in `index.html` matches the filename exactly

## Custom Domain (Optional)

If you want to use a custom domain (e.g., `dmp-neurips.com`):

1. Buy a domain from a registrar (GoDaddy, Namecheap, etc.)
2. Add a `CNAME` file to your repository with your domain name
3. Configure DNS settings at your registrar
4. Update GitHub Pages settings with custom domain

See: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

## Need Help?

- GitHub Pages Documentation: https://docs.github.com/en/pages
- GitHub Support: https://support.github.com
- HTML/CSS Issues: Check browser console (F12)

---

Good luck with your deployment! 🚀
