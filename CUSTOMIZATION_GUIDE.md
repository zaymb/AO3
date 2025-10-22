# AO3 Skin Customization Guide

This guide will help you customize your AO3 skin to match your personal preferences.

## Getting Started

Both `base-theme.css` and `dark-mode.css` use CSS variables at the top of the file. These make customization easy - just change the values in the `:root` section!

## Quick Customization: CSS Variables

### Colors

Change the color scheme by modifying these variables:

```css
:root {
  --primary-color: #990000;      /* Main brand color (red) */
  --link-color: #990000;          /* Link color */
  --link-hover-color: #cc0000;    /* Link hover color */
  --accent-color: #477d99;        /* Accent color (blue) */
  --background-color: #ffffff;    /* Page background */
  --text-color: #333333;          /* Main text color */
}
```

**Popular color schemes:**

**Cozy Brown:**
```css
--primary-color: #8b4513;
--link-color: #a0522d;
--accent-color: #daa520;
```

**Ocean Blue:**
```css
--primary-color: #006494;
--link-color: #247ba0;
--accent-color: #1b98e0;
```

**Purple Dream:**
```css
--primary-color: #7b2cbf;
--link-color: #9d4edd;
--accent-color: #c77dff;
```

### Typography

Change fonts and text size:

```css
:root {
  --font-body: 'Your Font Here', sans-serif;
  --font-heading: 'Your Heading Font', serif;
  --font-size-base: 16px;         /* Base text size */
  --line-height-base: 1.6;        /* Line spacing */
}
```

**Popular font combinations:**

**Classic Serif:**
```css
--font-body: Georgia, 'Times New Roman', serif;
--font-heading: 'Playfair Display', serif;
```

**Modern Sans:**
```css
--font-body: 'Inter', 'Helvetica Neue', sans-serif;
--font-heading: 'Montserrat', sans-serif;
```

**Comfortable Reading:**
```css
--font-body: 'Literata', 'Charter', serif;
--font-size-base: 18px;
--line-height-base: 1.8;
```

### Layout

Adjust spacing and width:

```css
:root {
  --max-width: 1200px;           /* Maximum content width */
  --spacing-small: 8px;
  --spacing-medium: 16px;
  --spacing-large: 24px;
  --border-radius: 4px;          /* Rounded corners */
}
```

**Layout presets:**

**Wide Layout:**
```css
--max-width: 1600px;
```

**Narrow Reading:**
```css
--max-width: 900px;
```

**Extra Cozy (more padding):**
```css
--spacing-small: 12px;
--spacing-medium: 20px;
--spacing-large: 32px;
```

## Common Customizations

### 1. Change Work Card Appearance

Make work listings more compact:
```css
.work.blurb {
  padding: 12px !important;
  margin-bottom: 8px !important;
}
```

Add more visual separation:
```css
.work.blurb {
  border: 2px solid var(--border-color) !important;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1) !important;
}
```

### 2. Customize Reading Experience

Increase text size for comfortable reading:
```css
#workskin {
  font-size: 1.3em !important;
  line-height: 2.0 !important;
  max-width: 700px !important;
}
```

Center-align paragraphs (instead of justify):
```css
.chapter .userstuff p {
  text-align: left !important;
}
```

Add paragraph spacing:
```css
.chapter .userstuff p {
  margin-bottom: 1.5em !important;
}
```

### 3. Tag Styling

Change tag appearance:
```css
.tag {
  background-color: var(--accent-color) !important;
  color: white !important;
  border-radius: 4px !important;
  padding: 6px 12px !important;
  font-weight: 600 !important;
}
```

### 4. Hide Elements

Hide kudos count on work listings:
```css
.kudos {
  display: none !important;
}
```

Hide hit counts:
```css
.hits {
  display: none !important;
}
```

Hide header image:
```css
#header .primary h1 {
  background-image: none !important;
}
```

### 5. Mobile Optimizations

Add to the bottom of your CSS for better mobile experience:
```css
@media (max-width: 768px) {
  #main {
    padding: 12px !important;
  }

  .work.blurb {
    padding: 12px !important;
  }

  #workskin {
    font-size: 1em !important;
    padding: 12px !important;
  }
}
```

## Advanced Customizations

### Custom Fonts from Google Fonts

1. Find your font at [Google Fonts](https://fonts.google.com/)
2. Add this at the TOP of your CSS file:

```css
@import url('https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700&display=swap');
```

3. Use the font in your variables:
```css
--font-body: 'Merriweather', serif;
```

### Background Patterns

Add a subtle background pattern:
```css
body {
  background-image: url('https://www.transparenttextures.com/patterns/paper.png') !important;
  background-repeat: repeat !important;
}
```

### Custom Work Type Colors

Color-code different work types:
```css
/* Color for completed works */
dt.status:contains("Complete") + dd {
  color: #4caf50 !important;
}

/* Color for in-progress works */
dt.status:contains("In-Progress") + dd {
  color: #ff9800 !important;
}
```

## Testing Your Changes

1. Make changes to the CSS file
2. Copy the entire content
3. In AO3: Go to **My Preferences** > **Skins** > Edit your skin
4. Paste and save
5. Refresh any AO3 page to see changes

**Tip:** Keep the AO3 skin editor open in one tab and browse AO3 in another tab. Make changes, save, and refresh to see results immediately!

## Troubleshooting

### Changes aren't showing up
- Clear your browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Make sure you saved the skin in AO3 preferences
- Check that the skin is selected in your preferences

### Styles look broken
- Check for syntax errors (missing semicolons, brackets)
- Make sure all `!important` flags are present
- Validate your CSS at [CSS Validator](https://jigsaw.w3.org/css-validator/)

### Want to reset?
Copy the original `base-theme.css` or `dark-mode.css` from this repository again.

## Inspiration & Resources

- [AO3 Skins Tutorial](https://archiveofourown.org/faq/skins-and-archive-interface)
- [Color Palette Generator](https://coolors.co/)
- [Google Fonts](https://fonts.google.com/)
- [CSS Color Picker](https://htmlcolorcodes.com/)

## Sharing Your Skin

If you create a skin you love, consider:
1. Posting it on AO3 as a public skin
2. Sharing the code on Tumblr/Twitter with #AO3Skins
3. Creating a fork of this repository with your customization

Happy customizing!
