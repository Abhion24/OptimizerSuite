# Deployment Guide for PC Optimizer Suite Website

This guide will help you deploy your website to GitHub Pages.

## Prerequisites

1. A GitHub account (you already have one: https://github.com/Abhion24)
2. Git installed on your computer

## Steps to Deploy

### 1. Create a New Repository

1. Go to https://github.com/new
2. Name your repository (e.g., `optimizer-website` or `pc-optimizer-suite`)
3. Make it public (required for GitHub Pages)
4. Do NOT initialize with a README
5. Click "Create repository"

### 2. Push Your Code to GitHub

Open a terminal/command prompt in your project directory and run:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/Abhion24/[your-repo-name].git
git push -u origin main
```

Replace `[your-repo-name]` with the name of your repository.

### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to the "Pages" section
4. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click "Save"
6. Wait a minute for GitHub to build your site

### 4. View Your Website

After a minute or so, your website will be available at:
`https://Abhion24.github.io/[your-repo-name]/`

## Troubleshooting

### If CSS is not loading:

1. Make sure all paths in your HTML are relative (not starting with `/`)
2. Check that your CSS file is in the `css/` directory
3. Verify that your repository structure matches your local structure

### If images are not loading:

1. Ensure all image paths are relative
2. Check that your images are in the `images/` directory

### If download link doesn't work:

1. Make sure your installer is in the `downloads/` directory
2. Verify the filename matches exactly (case-sensitive)

## Updating Your Website

To update your website after making changes:

1. Make your changes locally
2. Test them locally by running a local server:
   ```bash
   python -m http.server 8000
   ```
3. Open http://localhost:8000 in your browser to test
4. Commit and push your changes:
   ```bash
   git add .
   git commit -m "Description of changes"
   git push
   ```

GitHub Pages will automatically update your website within a minute or two.

## Custom Domain (Optional)

If you want to use a custom domain:

1. In your repository settings, go to "Pages"
2. Under "Custom domain", enter your domain
3. Follow the instructions to configure DNS records with your domain provider

Note: Custom domains require additional configuration and may take some time to propagate.