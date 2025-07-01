# Deploy Portfolio to GitHub Pages

Follow these steps to deploy your portfolio website to GitHub Pages:

## Step 1: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in to your account
2. Click the "+" icon in the top right corner and select "New repository"
3. Name your repository: `portfolio` or `gopi-palepu-portfolio`
4. Make it **Public** (required for free GitHub Pages)
5. **DO NOT** initialize with README, .gitignore, or license (we already have these)
6. Click "Create repository"

## Step 2: Connect Your Local Repository to GitHub

After creating the repository, GitHub will show you commands. Run these in your terminal:

```bash
# Add the remote repository (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/portfolio.git

# Push your code to GitHub
git branch -M main
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to "Pages" section (in the left sidebar)
4. Under "Source", select "Deploy from a branch"
5. Under "Branch", select "main" and click "Save"
6. Your site will be available at: `https://YOUR_USERNAME.github.io/portfolio`

## Step 4: Custom Domain (Optional)

If you want to use a custom domain:

1. In the Pages settings, enter your domain in the "Custom domain" field
2. Add a CNAME file to your repository with your domain name
3. Configure your DNS settings to point to GitHub Pages

## Step 5: Update Meta Tags

After deployment, update the meta tags in `index.html`:

```html
<!-- Replace with your actual GitHub Pages URL -->
<meta property="og:url" content="https://YOUR_USERNAME.github.io/portfolio/">
<meta property="twitter:url" content="https://YOUR_USERNAME.github.io/portfolio/">
```

## Troubleshooting

### If you get authentication errors:
1. Use GitHub CLI: `gh auth login`
2. Or use Personal Access Token
3. Or use SSH keys

### If the site doesn't load:
1. Check the repository is public
2. Wait a few minutes for GitHub Pages to build
3. Check the Actions tab for any build errors

### To update your site:
```bash
git add .
git commit -m "Update portfolio content"
git push
```

## Quick Commands

Here are the commands you need to run (replace YOUR_USERNAME):

```bash
# Add remote repository
git remote add origin https://github.com/YOUR_USERNAME/portfolio.git

# Push to GitHub
git branch -M main
git push -u origin main
```

Your portfolio will be live at: `https://YOUR_USERNAME.github.io/portfolio` 