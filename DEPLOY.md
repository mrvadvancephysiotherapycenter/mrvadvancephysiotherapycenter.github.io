# Deployment Instructions for GitHub Pages

## Step 1: Create GitHub Repository

1. Go to https://github.com/new
2. Repository name: `mrv-physiotherapy-website` (or any name you prefer)
3. Description: "MRV Advance Physiotherapy Center - Official Website"
4. Set to **Public** (required for free GitHub Pages)
5. **DO NOT** initialize with README, .gitignore, or license (we already have these)
6. Click "Create repository"

## Step 2: Push Code to GitHub

Run these commands in the terminal (from the `mrv-physiotherapy-website` directory):

```bash
cd /Users/arunkumarm/vmware_git/arun-work/mrv-physiotherapy-website

# Add the remote repository (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/arunkumarmurugesan/mrv-physiotherapy-website.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings** tab
3. Scroll down to **Pages** section (left sidebar)
4. Under **Source**, select **Deploy from a branch**
5. Select **main** branch and **/ (root)** folder
6. Click **Save**

## Step 4: Access Your Website

Your website will be available at:
- **GitHub Pages URL**: `https://arunkumarmurugesan.github.io/mrv-physiotherapy-website/`
- It may take a few minutes to be live after enabling Pages

## Step 5: Custom Domain (Optional - if you renew mrvphysiotherapycenter.com)

If you want to use your custom domain `mrvphysiotherapycenter.com`:

1. In GitHub repository Settings → Pages
2. Under **Custom domain**, enter: `mrvphysiotherapycenter.com`
3. Add a file named `CNAME` in the root directory with content:
   ```
   mrvphysiotherapycenter.com
   ```
4. Update your domain's DNS settings:
   - Add an A record pointing to GitHub Pages IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - OR add a CNAME record pointing to: `arunkumarmurugesan.github.io`

## Notes

- The `.nojekyll` file is included to ensure GitHub Pages serves all files correctly
- After pushing, wait 1-2 minutes for the site to be live
- Any future changes: just commit and push to update the live site

