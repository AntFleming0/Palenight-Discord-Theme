# Customization Guide

This guide provides detailed instructions for customizing the VSCode Palenight theme for BetterDiscord.

---

## Table of Contents

- [Quick Start](#quick-start)
- [Color Customization](#color-customization)
- [Typography Customization](#typography-customization)
- [Layout & Spacing](#layout--spacing)
- [Background Images](#background-images)
- [Advanced Customization](#advanced-customization)
- [Examples](#examples)

---

## Quick Start

To customize the theme, add your custom CSS variables after the `@import` statement in your theme file:

```css
@import url("https://antfleming0.github.io/BetterDiscordTheme/theme.css");

:root {
  /* Your customizations here */
}
```

---

## Color Customization

### Primary Accent Colors

```css
:root {
  /* Main accent (used for links, selections, focus states) */
  --accent-primary: #82aaff;
  --accent-primary-hover: #a3bfff;
  --accent-primary-active: #6c8fdb;

  /* Secondary accent (used for special elements) */
  --accent-secondary: #c792ea;
  --accent-secondary-hover: #d7a6f0;
  --accent-secondary-active: #b67cd1;

  /* Tertiary accent (used for highlights) */
  --accent-tertiary: #89ddff;
  --accent-tertiary-hover: #a8e6ff;
  --accent-tertiary-active: #6dc4e6;
}
```

### Background Colors

```css
:root {
  /* Background scale (darkest to lightest) */
  --bg-darkest: #292d3e; /* Main background */
  --bg-darker: #2b2f3e; /* Slightly lighter */
  --bg-dark: #2f3347; /* Sidebar */
  --bg-medium: #32374a; /* Cards, elevated elements */
  --bg-light: #3a3f58; /* Hover states */
  --bg-lighter: #444a67; /* Active states */
}
```

### Text Colors

```css
:root {
  --text-primary: #a6accd; /* Main text */
  --text-secondary: #959dcb; /* Secondary text */
  --text-muted: #676e95; /* Muted/disabled text */
  --text-bright: #ffffff; /* Emphasized text */
  --text-dimmed: #4e5579; /* Very dim text */
}
```

### Status Colors

```css
:root {
  --status-online: #c3e88d; /* Online status */
  --status-idle: #ffcb6b; /* Idle/away */
  --status-dnd: #f07178; /* Do not disturb */
  --status-offline: #676e95; /* Offline */
  --status-streaming: #c792ea; /* Streaming */
}
```

### Syntax Highlighting Colors

```css
:root {
  --color-keyword: #c792ea; /* Purple - keywords */
  --color-string: #c3e88d; /* Green - strings */
  --color-function: #82aaff; /* Blue - functions */
  --color-variable: #ffcb6b; /* Yellow - variables */
  --color-comment: #676e95; /* Gray - comments */
  --color-operator: #89ddff; /* Cyan - operators */
  --color-property: #f07178; /* Red - properties */
  --color-number: #f78c6c; /* Orange - numbers */
}
```

---

## Typography Customization

### Font Families

```css
:root {
  /* Primary font for UI */
  --font-primary: Consolas, "Courier New", "Monaco", monospace;

  /* Display font for headings */
  --font-display: Consolas, "Courier New", monospace;

  /* Code blocks and inline code */
  --font-code: Consolas, "Courier New", "Source Code Pro", monospace;

  /* Alternative fonts */
  --font-sans: "Segoe UI", "Helvetica Neue", Arial, sans-serif;
  --font-mono: "Fira Code", "Source Code Pro", "JetBrains Mono", monospace;
}
```

### Font Sizes

```css
:root {
  --font-size-xs: 11px;
  --font-size-sm: 12px;
  --font-size-base: 14px; /* Default size */
  --font-size-md: 15px;
  --font-size-lg: 16px;
  --font-size-xl: 18px;
  --font-size-xxl: 20px;
  --font-size-display: 24px;
}
```

### Font Weights

```css
:root {
  --font-weight-light: 300;
  --font-weight-normal: 400;
  --font-weight-medium: 500;
  --font-weight-semibold: 600;
  --font-weight-bold: 700;
}
```

### Line Heights

```css
:root {
  --line-height-tight: 1.2;
  --line-height-base: 1.4;
  --line-height-relaxed: 1.6;
  --line-height-loose: 1.8;
}
```

---

## Layout & Spacing

### Spacing Scale

```css
:root {
  --spacing-xs: 4px;
  --spacing-sm: 8px;
  --spacing-md: 12px;
  --spacing-lg: 16px;
  --spacing-xl: 24px;
  --spacing-xxl: 32px;
}
```

### Border Radius

```css
:root {
  --radius-sm: 2px;
  --radius-md: 4px;
  --radius-lg: 8px;
  --radius-xl: 12px;
  --radius-round: 50%; /* Perfect circles */
}
```

### Borders

```css
:root {
  --border-default: rgba(0, 0, 0, 0.2);
  --border-subtle: rgba(0, 0, 0, 0.1);
  --border-strong: rgba(0, 0, 0, 0.3);
  --border-accent: var(--accent-primary);
}
```

### Shadows

```css
:root {
  --shadow-sm: 0 1px 2px rgba(0, 0, 0, 0.3);
  --shadow-md: 0 2px 4px rgba(0, 0, 0, 0.4);
  --shadow-lg: 0 4px 8px rgba(0, 0, 0, 0.5);
  --shadow-xl: 0 8px 16px rgba(0, 0, 0, 0.6);
}
```

---

## Background Images

### Adding a Custom Background

```css
:root {
  /* Your image URL (must be HTTPS) */
  --custom-background-image: url("https://example.com/image.jpg");

  /* Blur amount (0-20px recommended) */
  --custom-background-blur: 5px;

  /* Opacity (0-1) */
  --custom-background-opacity: 0.3;
}
```

### Removing Background Image

```css
:root {
  --custom-background-image: none;
}
```

---

## Advanced Customization

### Transition Speeds

```css
:root {
  --transition-fast: 0.1s ease;
  --transition-normal: 0.2s ease;
  --transition-slow: 0.3s ease;
}
```

### Focus States

```css
:root {
  --focus-ring: var(--accent-primary);
  --focus-glow: 0 0 0 2px rgba(130, 170, 255, 0.4);
}
```

### Overlays

```css
:root {
  --overlay-dark: rgba(0, 0, 0, 0.5);
  --overlay-darker: rgba(0, 0, 0, 0.7);
  --overlay-light: rgba(255, 255, 255, 0.05);
  --overlay-lighter: rgba(255, 255, 255, 0.1);
}
```

---

## Examples

### Example 1: Pink Accent Theme

```css
@import url("https://antfleming0.github.io/BetterDiscordTheme/theme.css");

:root {
  --accent-primary: #ff6b9d;
  --accent-primary-hover: #ff8bb0;
  --accent-primary-active: #e6548a;
  --accent-secondary: #b4e1ff;
  --accent-tertiary: #ffb4e6;
}
```

### Example 2: Larger Text

```css
@import url("https://antfleming0.github.io/BetterDiscordTheme/theme.css");

:root {
  --font-size-base: 16px;
  --font-size-sm: 14px;
  --font-size-xs: 12px;
  --line-height-base: 1.6;
}
```

### Example 3: Custom Background

```css
@import url("https://antfleming0.github.io/BetterDiscordTheme/theme.css");

:root {
  --custom-background-image: url("https://images.unsplash.com/photo-1557683316-973673baf926");
  --custom-background-blur: 8px;
  --custom-background-opacity: 0.25;
}
```

### Example 4: Different Font

```css
@import url("https://antfleming0.github.io/BetterDiscordTheme/theme.css");

@import url("https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;500;600&display=swap");

:root {
  --font-primary: "Fira Code", monospace;
  --font-code: "Fira Code", monospace;
}
```

### Example 5: More Rounded Corners

```css
@import url("https://antfleming0.github.io/BetterDiscordTheme/theme.css");

:root {
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
  --radius-xl: 16px;
}
```

### Example 6: Compact Spacing

```css
@import url("https://antfleming0.github.io/BetterDiscordTheme/theme.css");

:root {
  --spacing-xs: 2px;
  --spacing-sm: 4px;
  --spacing-md: 8px;
  --spacing-lg: 12px;
  --spacing-xl: 16px;
  --spacing-xxl: 24px;
}
```

---

## Tips & Best Practices

1. **Start Small**: Customize one aspect at a time and test thoroughly
2. **Use Color Pickers**: Tools like [Coolors](https://coolors.co/) help create cohesive palettes
3. **Test in Different Lighting**: Check your theme in various lighting conditions
4. **Consider Accessibility**: Maintain sufficient color contrast for readability
5. **Back Up Your Customizations**: Save your custom CSS in a separate file
6. **Test with Plugins**: Verify your customizations work with your favorite plugins

---

## Need Help?

- Check the [main README](README.md) for troubleshooting
- Open an [issue on GitHub](https://github.com/AntFleming0/BetterDiscordTheme/issues)
- Share your customizations with the community!

---

**Happy customizing!** 🎨
