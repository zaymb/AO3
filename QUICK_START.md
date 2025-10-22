# Quick Start Guide

Get your custom AO3 skin up and running in 5 minutes!

## Step 1: Choose Your Skin

Pick one of the pre-made skins:
- **base-theme.css** - Clean, modern light theme
- **dark-mode.css** - Comfortable dark theme for night reading

## Step 2: Install on AO3

### Method A: AO3 Site Skin (Recommended)

1. **Copy the CSS**
   - Open the skin file you want (e.g., `skins/dark-mode.css`)
   - Copy ALL the content (Ctrl+A, Ctrl+C)

2. **Create the Skin on AO3**
   - Log into your AO3 account
   - Go to: **My Preferences** → **Skins** → **Create Site Skin**
   - Title: Give it a name (e.g., "My Dark Theme")
   - CSS: Paste the copied CSS code
   - Click **Submit**

3. **Activate Your Skin**
   - Go back to: **My Preferences** → **Skins**
   - Under "Choose a skin", select your newly created skin
   - Click **Update Preferences**

4. **Done!** Refresh any AO3 page to see your new theme

### Method B: Browser Extension (Stylus)

1. **Install Stylus**
   - [Chrome/Edge](https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne)
   - [Firefox](https://addons.mozilla.org/en-US/firefox/addon/styl-us/)

2. **Create a New Style**
   - Click the Stylus extension icon
   - Click "Manage" → "Write new style"

3. **Add the Code**
   - Copy all content from your chosen skin file
   - Paste into the code editor
   - Under "Applies to", select "URLs on the domain"
   - Enter: `archiveofourown.org`
   - Name your style (e.g., "AO3 Dark Mode")
   - Click **Save**

4. **Done!** Refresh AO3 to see changes

## Step 3: Customize (Optional)

Want to tweak colors or fonts? Check out the **CSS Variables** section at the top of your skin file:

```css
:root {
  --primary-color: #990000;    /* Change this to your favorite color! */
  --font-size-base: 16px;      /* Make text bigger or smaller */
  --max-width: 1200px;         /* Adjust content width */
}
```

Just change the values, save, and refresh AO3 to see your changes!

## Troubleshooting

**Changes not showing?**
- Clear browser cache (Ctrl+Shift+R / Cmd+Shift+R)
- Make sure skin is selected in AO3 preferences
- Check that you saved the skin

**Looks broken?**
- Check for copy/paste errors
- Make sure you copied the ENTIRE file
- Try the other installation method

**Need help?**
- Check the detailed [CUSTOMIZATION_GUIDE.md](CUSTOMIZATION_GUIDE.md)
- Read the [README.md](README.md) for more info

## Next Steps

- Browse [CUSTOMIZATION_GUIDE.md](CUSTOMIZATION_GUIDE.md) for detailed customization options
- Mix and match components from `skins/components/` folder
- Share your custom theme with friends!

Happy reading!
