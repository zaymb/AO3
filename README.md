# AO3 Custom WebUI Styles

Personal custom CSS styles for Archive of Our Own (AO3).

## Quick Start

### Method 1: AO3 Site Skins (Recommended)

1. Log into your AO3 account
2. Go to **My Preferences** > **Skins** > **Create Site Skin**
3. Copy the CSS from `skins/` folder
4. Paste into the CSS field
5. Click **Submit**
6. Go back to **My Preferences** and select your new skin

### Method 2: Browser Extension (Stylus)

1. Install [Stylus](https://github.com/openstyles/stylus) extension
2. Click the Stylus icon > **Manage**
3. Click **Write new style**
4. Copy CSS from `skins/` folder
5. Set "Applies to" > "URLs on the domain" > `archiveofourown.org`
6. Save

## Project Structure

```
skins/
  ├── base-theme.css          # Main custom theme
  ├── dark-mode.css           # Dark mode variant
  └── components/             # Modular components
      ├── work-card.css       # Work listing styles
      ├── reading-view.css    # Work reading experience
      └── navigation.css      # Header/footer styles
```

## Customization Tips

### Common Customizations

- **Font changes**: Modify `font-family` properties
- **Color scheme**: Update CSS variables in `:root`
- **Layout width**: Adjust `max-width` on containers
- **Spacing**: Modify `padding` and `margin` values

### CSS Selectors Reference

- `#main` - Main content area
- `.work` - Individual work listings
- `.navigation` - Top navigation
- `.header` - Page headers
- `#workskin` - Work text content

## Resources

- [AO3 Skin Help](https://archiveofourown.org/faq/skins-and-archive-interface)
- [AO3 Parent Skins](https://archiveofourown.org/skins)
- [CSS Documentation](https://developer.mozilla.org/en-US/docs/Web/CSS)

## Contributing

This is a personal skin repository, but feel free to fork and modify for your own use!
