# VSCode Palenight Theme for BetterDiscord

A professional, modular BetterDiscord theme heavily inspired by Visual Studio Code's Palenight (Mild Contrast) color scheme. Features custom loading screens, three theme variants, and extensive customization options.

![Theme Preview](assets/screenshots/preview.png)
_Screenshots coming soon!_

---

## ✨ Features

- 🎨 **Three Beautiful Variants**: Palenight (default), Dark (higher contrast), and Light
- 💻 **VSCode-Inspired Design**: Familiar color palette and typography for developers
- ⚡ **Custom Loading Screen**: Code animation effect inspired by VSCode
- 🔤 **Consolas Typography**: Monospace font system for a clean, code-editor feel
- 🎭 **Smooth Animations**: Subtle transitions and hover effects (200-300ms)
- 📦 **Modular Architecture**: Clean, organized CSS modules for easy customization
- 🎯 **Custom Scrollbars**: Thin, VSCode-style scrollbars
- 🔧 **Highly Customizable**: Extensive CSS variables for colors, spacing, fonts, and more
- ♿ **Accessible**: Respects `prefers-reduced-motion` settings
- 🔌 **Plugin Compatible**: Tested with popular BetterDiscord plugins

---

## 📥 Installation

### Step 1: Install BetterDiscord

If you haven't already, install [BetterDiscord](https://betterdiscord.app/):

1. Download BetterDiscord from the official website
2. Run the installer
3. Select Discord Stable, PTB, or Canary
4. Restart Discord

### Step 2: Install the Theme

**Method 1: Direct Import (Recommended)**

1. Open Discord Settings (gear icon)
2. Go to **Themes** under BetterDiscord
3. Click **Open Theme Folder**
4. Create a new file called `VSCodePalenight.theme.css`
5. Open the file in a text editor and paste the following:

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

6. Save the file
7. Go back to Discord Settings → Themes
8. Enable "VSCode Palenight"

**Method 2: Download from GitHub**

1. Go to [GitHub Releases](https://github.com/AntFleming0/BetterDiscordTheme/releases)
2. Download `theme.css` (or variant files)
3. Place the file in your BetterDiscord themes folder
4. Enable in Discord Settings → Themes

---

## 🎨 Theme Variants

### Palenight (Default)

The authentic VSCode Palenight (Mild Contrast) experience.

```css
@import url("https://antfleming0.github.io/BetterDiscordTheme/theme.css");
```

### Dark (Higher Contrast)

A darker variant with increased contrast for better readability.

```css
@import url("https://antfleming0.github.io/BetterDiscordTheme/theme-dark.css");
```

### Light

A light theme for those who prefer bright environments.

```css
@import url("https://antfleming0.github.io/BetterDiscordTheme/theme-light.css");
```

To switch variants, simply change the `@import` URL in your theme file!

---

## 🔧 Customization

The theme is highly customizable using CSS variables. Add your customizations after the `@import` statement:

```css
@import url("https://antfleming0.github.io/BetterDiscordTheme/theme.css");

/* Your customizations */
:root {
  /* Change accent color */
  --accent-primary: #ff6b9d;
  --accent-secondary: #b4e1ff;

  /* Add background image */
  --custom-background-image: url("https://example.com/your-image.jpg");
  --custom-background-blur: 5px;
  --custom-background-opacity: 0.3;

  /* Change fonts */
  --font-primary: "Fira Code", monospace;

  /* Adjust spacing */
  --spacing-md: 16px;
  --border-radius-md: 8px;
}
```

### Available Customization Variables

#### Colors

- `--accent-primary` - Main accent color (default: #82AAFF)
- `--accent-secondary` - Secondary accent (default: #C792EA)
- `--accent-tertiary` - Tertiary accent (default: #89DDFF)
- `--bg-darkest` - Main background
- `--text-primary` - Primary text color

#### Typography

- `--font-primary` - Main font (default: Consolas)
- `--font-code` - Code font
- `--font-size-base` - Base font size (default: 14px)

#### Spacing & Layout

- `--spacing-xs` through `--spacing-xxl` - Spacing scale
- `--radius-sm` through `--radius-xl` - Border radius scale

#### Custom Background

- `--custom-background-image` - Your background image URL
- `--custom-background-blur` - Blur amount (px)
- `--custom-background-opacity` - Opacity (0-1)

For a complete list, see [CUSTOMIZATION.md](CUSTOMIZATION.md)

---

## 📸 Screenshots

### Palenight Variant

![Palenight](assets/screenshots/palenight.png)

### Dark Variant

![Dark](assets/screenshots/dark.png)

### Light Variant

![Light](assets/screenshots/light.png)

### Custom Loading Screen

![Loading](assets/screenshots/loading.png)

_Screenshots coming soon!_

---

## 🐛 Troubleshooting

### Theme doesn't load

- Ensure BetterDiscord is properly installed
- Check that the theme file has `.theme.css` extension
- Verify the theme is enabled in Discord Settings → Themes
- Try restarting Discord

### Colors look wrong

- Make sure you're using the correct variant
- Clear Discord cache (Ctrl+Shift+R or Cmd+Shift+R)
- Check for conflicting themes or CSS snippets

### Fonts not displaying correctly

- Ensure Consolas is installed on your system (it's included with Windows)
- On macOS/Linux, the theme will fall back to Courier New or Monaco
- You can customize the font in your theme file

### Performance issues

- Reduce `--custom-background-blur` or remove background image
- Enable "Reduced Motion" in your OS accessibility settings
- Disable other themes or heavy plugins

---

## 🔌 Plugin Compatibility

Tested and compatible with:

- ✅ BetterRoleColors
- ✅ MessageLoggerV2
- ✅ ReadAllNotificationsButton
- ✅ ChannelTabs
- ✅ OldTitleBar

If you encounter issues with a specific plugin, please [open an issue](https://github.com/AntFleming0/BetterDiscordTheme/issues).

---

## 📦 Repository Structure

```
BetterDiscordTheme/
├── src/
│   ├── modules/
│   │   ├── base.css              # Foundation styles & resets
│   │   ├── colors.css            # Palenight color palette
│   │   ├── typography.css        # Font system
│   │   ├── components.css        # Discord UI components
│   │   ├── animations.css        # Transitions & animations
│   │   └── loading-screen.css    # Custom loading screen
│   └── variants/
│       ├── palenight.css         # Default variant
│       ├── dark.css              # Dark variant
│       └── light.css             # Light variant
├── assets/
│   └── screenshots/              # Theme screenshots
├── theme.css                     # Main theme (Palenight)
├── theme-dark.css                # Dark variant
├── theme-light.css               # Light variant
├── README.md                     # This file
├── CUSTOMIZATION.md              # Detailed customization guide
├── LICENSE                       # MIT License
└── .gitignore
```

---

## 🤝 Contributing

Contributions are welcome! If you'd like to improve the theme:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Credits

- **VSCode Palenight Theme** - Original color scheme inspiration
- **[ClearVision](https://github.com/ClearVision/ClearVision-v7)** - Reference for BetterDiscord theme structure
- **[System24](https://github.com/refact0r/system24)** - Inspiration for loading screen animations
- **Material Theme** - Additional design inspiration

---

## 💬 Support & Community

- 🐛 [Report Issues](https://github.com/AntFleming0/BetterDiscordTheme/issues)
- 💡 [Request Features](https://github.com/AntFleming0/BetterDiscordTheme/issues/new)
- ⭐ [Star on GitHub](https://github.com/AntFleming0/BetterDiscordTheme)

---

## 📝 Changelog

### Version 1.0.0 (Initial Release)

- ✨ Three theme variants (Palenight, Dark, Light)
- 🎨 Complete VSCode Palenight color palette
- 💻 Consolas typography system
- ⚡ Custom loading screen with code animation
- 🎭 Smooth animations and transitions
- 📦 Modular CSS architecture
- 🔧 Extensive customization via CSS variables

---

**Made with ❤️ by AntFleming0**

**Enjoy your new VSCode-inspired Discord theme!** 🚀
