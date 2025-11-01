# GitHub Pages Setup Guide

This guide will help you set up GitHub Pages for your BetterDiscord theme.

## Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and log in with username: **AntFleming0**
2. Click the **+** icon in the top right and select **New repository**
3. Configure your repository:
   - **Repository name:** `BetterDiscordTheme`
   - **Description:** "VSCode Palenight theme for BetterDiscord - Professional theme inspired by Visual Studio Code"
   - **Visibility:** Choose Public (required for GitHub Pages free hosting)
   - **Initialize:** ✅ Add a README file (optional, we have one)
   - **Add .gitignore:** None (we have one)
   - **Choose a license:** MIT License (or use the LICENSE file we created)
4. Click **Create repository**

## Step 2: Upload Your Files to GitHub

### Option A: Using GitHub Web Interface (Easiest)

1. On your repository page, click **Add file** → **Upload files**
2. Drag and drop all these files/folders from your local directory:
   ```
   .gitignore
   LICENSE
   README.md
   CUSTOMIZATION.md
   index.html
   theme.css
   theme-dark.css
   theme-light.css
   src/ (entire folder)
   assets/ (entire folder)
   ```
3. Add a commit message: "Initial commit - VSCode Palenight theme v1.0.0"
4. Click **Commit changes**

### Option B: Using Git Command Line

Open PowerShell in your theme directory and run:

```powershell
# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit - VSCode Palenight theme v1.0.0"

# Add remote (replace with your repo URL)
git remote add origin https://github.com/AntFleming0/BetterDiscordTheme.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (tab at the top)
3. In the left sidebar, click **Pages** (under "Code and automation")
4. Under **Source**, select:
   - **Source:** Deploy from a branch
   - **Branch:** `main` (or `master`)
   - **Folder:** `/ (root)`
5. Click **Save**
6. Wait a few minutes for GitHub to build your site
7. Your site will be available at: `https://antfleming0.github.io/BetterDiscordTheme/`

## Step 4: Verify Your Theme Works

1. Visit: `https://antfleming0.github.io/BetterDiscordTheme/`
   - You should see the theme landing page
2. Test the theme file: `https://antfleming0.github.io/BetterDiscordTheme/theme.css`
   - You should see the CSS code
3. Test a module: `https://antfleming0.github.io/BetterDiscordTheme/src/modules/colors.css`
   - You should see the colors CSS

## Step 5: Install Your Theme in Discord

1. Open Discord Settings → Themes → Open Theme Folder
2. Create a new file: `VSCodePalenight.theme.css`
3. Add this content:

```css
/**
 * @name VSCode Palenight
 * @description VSCode-inspired Palenight theme
 * @author AntFleming0
 * @version 1.0.0
 * @source https://github.com/AntFleming0/BetterDiscordTheme
 */

@import url("https://antfleming0.github.io/BetterDiscordTheme/theme.css");
```

4. Save and enable the theme in Discord!

## Troubleshooting

### GitHub Pages Not Working

- **Wait:** It can take up to 10 minutes for the first deployment
- **Check Settings:** Make sure Pages is enabled in repository settings
- **Check Branch:** Ensure you selected the correct branch (main/master)
- **Check Files:** Make sure all files were uploaded correctly

### Theme Not Loading in Discord

- **HTTPS Required:** GitHub Pages automatically uses HTTPS (required by BetterDiscord)
- **Check URL:** Make sure you're using the exact GitHub Pages URL
- **Clear Cache:** Restart Discord with Ctrl+Shift+R (or Cmd+Shift+R on Mac)
- **Check Console:** Open Discord Developer Tools (Ctrl+Shift+I) and check for errors

### CSS Not Applying

- **Check Imports:** Make sure all @import statements use your GitHub Pages URL
- **Check File Paths:** URLs are case-sensitive on GitHub Pages
- **Test Individual Files:** Visit each CSS file URL directly to verify they load

## Making Changes

When you want to update your theme:

1. Make changes to your local files
2. Commit and push to GitHub:
   ```powershell
   git add .
   git commit -m "Description of changes"
   git push
   ```
3. GitHub Pages will automatically rebuild (takes 1-5 minutes)
4. Users will get the updates automatically (they may need to refresh Discord)

## Custom Domain (Optional)

If you want to use a custom domain like `palenight.yourdomain.com`:

1. Buy a domain name
2. In your repository Settings → Pages, enter your custom domain
3. Configure your domain's DNS settings to point to GitHub Pages
4. Update all @import URLs in your theme files to use the custom domain

## Additional Tips

- **Version Your Releases:** Use GitHub Releases to tag stable versions
- **Branch Strategy:** Use a `dev` branch for development, `main` for stable releases
- **Test Before Pushing:** Always test your theme locally before pushing updates
- **Backup:** Keep backups of working versions before making major changes

## Need Help?

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Support](https://support.github.com/)
- [BetterDiscord Documentation](https://docs.betterdiscord.app/)

---

**Your theme is now live!** 🎉

Share it with the community:

- https://antfleming0.github.io/BetterDiscordTheme/
- https://github.com/AntFleming0/BetterDiscordTheme
