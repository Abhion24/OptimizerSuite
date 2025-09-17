# PC Optimizer Suite Website

A minimalist dark/gray themed website for the PC Optimizer Suite Windows software.

## Deployment to GitHub Pages

To deploy this website to GitHub Pages, follow these steps:

1. Create a new repository on GitHub (e.g., `optimizer-website`)
2. Push this code to your repository
3. Go to your repository settings
4. Scroll down to the "Pages" section
5. Under "Source", select "Deploy from a branch"
6. Select "main" branch and "/ (root)" folder
7. Click "Save"
8. Your website will be available at `https://[your-username].github.io/[repository-name]/`

## File Structure

```
├── css/
│   └── styles.css          # All styling
├── downloads/
│   └── OptimizerSetup.exe  # Software installer
├── images/
│   ├── toolkit1.png        # Screenshot placeholder
│   ├── toolkit2.png        # Screenshot placeholder
│   └── toolkit3.png        # Screenshot placeholder
├── js/
│   └── config.js           # Configuration for GitHub Pages
├── index.html              # Main webpage
└── README.md               # This file
```

## Notes

- All paths in the HTML and CSS files are relative, which makes them work correctly with GitHub Pages
- The download link points to the actual installer file in the downloads directory
- The website is fully responsive and works on mobile, tablet, and desktop devices

## Customization

To customize this website for your own software:
1. Replace the placeholder images in the `images/` directory
2. Update the text content in `index.html`
3. Replace `OptimizerSetup.exe` with your actual installer
4. Update the version information in the download section