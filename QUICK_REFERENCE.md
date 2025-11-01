# 🚀 Quick Reference Card

## GitHub Setup (5 Steps)

1. **Create repo:** github.com → New repository → Name: `BetterDiscordTheme` → Public → Create
2. **Upload files:** Drag all files/folders to GitHub (or use git commands)
3. **Enable Pages:** Settings → Pages → Source: main branch → Save
4. **Wait:** 5-10 minutes for deployment
5. **Live at:** `https://antfleming0.github.io/BetterDiscordTheme/`

## Install Theme in Discord

```css
/**
 * @name VSCode Palenight
 * @author AntFleming0
 * @version 1.0.0
 */

@import url("https://antfleming0.github.io/BetterDiscordTheme/theme.css");
```

Save as: `VSCodePalenight.theme.css` in Discord themes folder

## Theme Variants URLs

- **Palenight:** `theme.css`
- **Dark:** `theme-dark.css`
- **Light:** `theme-light.css`

## Quick Customizations

```css
:root {
  /* Accent color */
  --accent-primary: #ff6b9d;

  /* Background image */
  --custom-background-image: url("IMAGE_URL");
  --custom-background-blur: 5px;

  /* Font */
  --font-primary: "Fira Code", monospace;

  /* Font size */
  --font-size-base: 16px;
}
```

## Important Files

- `GITHUB_SETUP.md` - Full GitHub instructions
- `PROJECT_SUMMARY.md` - Complete overview
- `README.md` - User documentation
- `CUSTOMIZATION.md` - All variables

## Git Commands (Optional)

```powershell
cd C:\Users\ImLush\Documents\BetterDiscordTheme
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/AntFleming0/BetterDiscordTheme.git
git branch -M main
git push -u origin main
```

## File Structure

```
BetterDiscordTheme/
├── theme.css (main)
├── theme-dark.css
├── theme-light.css
├── index.html
├── src/
│   ├── modules/ (6 files)
│   └── variants/ (3 files)
└── assets/screenshots/
```

## Your URLs (after GitHub Pages setup)

- **Website:** https://antfleming0.github.io/BetterDiscordTheme/
- **Theme:** https://antfleming0.github.io/BetterDiscordTheme/theme.css
- **Repo:** https://github.com/AntFleming0/BetterDiscordTheme

## Need Help?

1. Check `PROJECT_SUMMARY.md`
2. Check `GITHUB_SETUP.md`
3. Check other .md files
4. GitHub Docs: docs.github.com/en/pages

---

**Everything is ready to go!** 🎉
