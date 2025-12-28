# Deployment Guide

## GitHub Pages

1. Go to repository Settings
2. Navigate to Pages section
3. Select branch: `main`
4. Select folder: `/ (root)`
5. Click Save
6. Your site will be live at: `https://YOUR_USERNAME.github.io/random-joke-generator/`

## Netlify

1. Sign up at [Netlify](https://www.netlify.com/)
2. Click "New site from Git"
3. Connect your GitHub repository
4. Build settings: Leave empty (static site)
5. Click "Deploy site"

## Vercel

1. Sign up at [Vercel](https://vercel.com/)
2. Import your GitHub repository
3. Configure project (no build step needed)
4. Deploy

## Custom Server

Upload `index.html` to your web server's public directory.
```bash
# Example with SCP
scp index.html user@yourserver.com:/var/www/html/
```