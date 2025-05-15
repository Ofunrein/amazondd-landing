# Creating a GitHub Personal Access Token (PAT)

## Step 1: Access the Token Settings
1. Log in to your GitHub account
2. Click on your profile photo in the top-right corner
3. Select "Settings" from the dropdown menu
4. Scroll down and click on "Developer settings" in the left sidebar
5. Click on "Personal access tokens" in the left sidebar
6. Click on "Tokens (classic)"

## Step 2: Generate a New Token
1. Click on "Generate new token" button
2. Select "Generate new token (classic)"
3. Enter a descriptive name in the "Note" field (e.g., "Amazon DD Landing Page")
4. Set an expiration period (recommended: 30 days)

## Step 3: Select Token Permissions
For GitHub Pages deployments, you need:
- Select "repo" (Full control of private repositories)
- Select "workflow" (if you plan to use GitHub Actions)

## Step 4: Create the Token
1. Scroll to the bottom of the page
2. Click the "Generate token" button

## Step 5: Save Your Token
IMPORTANT: Copy your token immediately and save it in a secure location. GitHub will only show it once.

## Step 6: Use Your Token
When pushing to GitHub, use your token as the password when prompted. If using HTTPS:
```bash
# Set your username
git config --global user.name "YOUR_USERNAME"

# When prompted for a password, use your personal access token
git push -u origin gh-pages
```

You can also embed the token in the URL when setting the remote:
```bash
git remote set-url origin https://YOUR_USERNAME:YOUR_TOKEN@github.com/YOUR_USERNAME/amazondd-landing.git
```

For security, avoid storing your token in clear text in your git configuration. 