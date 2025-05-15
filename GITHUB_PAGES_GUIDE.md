# Step-by-Step Guide to Deploy to GitHub Pages

## 1. Create Repository on GitHub
1. Open your web browser and go to: https://github.com/new
2. Enter `amazondd-landing` as the repository name
3. Add a description like "Landing page for Amazon Designs & Decor"
4. Select "Public" for the repository visibility
5. Do NOT initialize with a README, .gitignore, or license
6. Click "Create repository"

## 2. Push Your Local Code to GitHub

Open your terminal and run the following commands, replacing `YOUR_USERNAME` with your actual GitHub username:

```bash
# Check which branches you have
git branch

# Make sure you're on the gh-pages branch
git checkout gh-pages

# Update remote origin with your actual GitHub username
git remote set-url origin https://github.com/YOUR_USERNAME/amazondd-landing.git

# Push to GitHub
git push -u origin gh-pages
```

When prompted, enter your GitHub username and password or personal access token.

## 3. Configure GitHub Pages in Repository Settings

1. Go to your repository on GitHub
2. Click on "Settings" in the top menu
3. Click on "Pages" in the left sidebar
4. Under "Source", select "Deploy from a branch"
5. Under "Branch", select "gh-pages" and "/ (root)"
6. Click "Save"

## 4. Wait for Deployment

GitHub will automatically build and deploy your site. This usually takes a few minutes.

## 5. Access Your Live Site

Once deployed, your site will be available at:
https://YOUR_USERNAME.github.io/amazondd-landing/

You can check the status of your deployment in the "Actions" tab of your repository.

If you make future changes, simply commit and push them to the gh-pages branch, and GitHub will automatically update your live site. 