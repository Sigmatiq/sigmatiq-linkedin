# SigmatiqAI Social Media Branding Package

Professional social media headers and profile images for SigmatiqAI, generated from HTML templates using Puppeteer at 2x resolution for high-quality output.

## Overview

This package contains HTML templates and an automated generation script to create consistent, professional social media assets for all major platforms.

### Brand Identity

- **Company Name:** SigmatiqAI
- **Username:** @SigmatiqAI (universal across platforms)
- **Tagline:** Your AI Trading Companion
- **Subtitle Line 1:** Built for Beginner Traders
- **Subtitle Line 2:** Earn While You Learn
- **Website:** https://sigmatiq.ai

### Brand Colors

```css
Teal (Primary):    #00C4A7
Golden (Accent):   #FFB800
Dark Background:   #0A1414
Card Background:   #152626
```

### Typography

- **Font:** Inter (Google Fonts)
- **Weights:** 300, 400, 500, 600, 700, 800, 900

## Directory Structure

```
social-media-branding/
├── templates/                        # HTML templates for each platform
│   ├── twitter-alert-behind-steps.html  # 1500x500px - Twitter/X header
│   ├── linkedin-with-alert.html         # 1128x191px - LinkedIn banner
│   ├── facebook-with-alert.html         # 820x312px - Facebook cover
│   ├── youtube-with-alert.html          # 2560x1440px - YouTube banner
│   ├── discord-with-alert.html          # 960x540px - Discord banner
│   └── profile-with-alert.html          # 800x800px - Profile picture
├── output/                           # Generated PNG files (2x resolution)
│   ├── twitter-header.png
│   ├── linkedin-banner.png
│   ├── facebook-cover.png
│   ├── youtube-banner.png
│   ├── discord-banner.png
│   └── profile-picture.png
├── package.json                      # Node.js dependencies
├── generate-headers.js               # Screenshot automation script
├── README.md                         # This file
├── DISCORD_COMMUNITY_GUIDELINES.md   # Discord server setup guide
└── REDDIT_POST_TEMPLATES.md          # Reddit posting strategy
```

## Quick Start

### 1. Install Dependencies

```bash
npm install
```

This will install Puppeteer and all required dependencies.

### 2. Generate All Headers

```bash
npm run generate:all
```

This generates all social media headers at 2x resolution in the `output/` directory.

### 3. Generate Individual Headers

```bash
# Twitter header (1500x500px)
npm run generate:twitter

# LinkedIn banner (1128x191px)
npm run generate:linkedin

# Facebook cover (820x312px)
npm run generate:facebook

# YouTube banner (2560x1440px)
npm run generate:youtube

# Profile picture (800x800px)
npm run generate:profile

# Discord banner (960x540px)
npm run generate:discord
```

## Template Specifications

### Twitter Header (1500x500px)
- **File:** `templates/twitter-alert-behind-steps.html`
- **Output:** `output/twitter-header.png`
- **Dimensions:** 1500x500px
- **Resolution:** 2x (3000x1000px actual)
- **Features:**
  - Logo and brand name on left with taglines
  - Options alert card (AAPL 190C example) with metrics and buttons
  - Process flow (Paper → Practice → Live) inside alert card
  - Dark gradient background with subtle grid and orbs
  - Teal and golden accent colors

### LinkedIn Banner (1128x191px)
- **File:** `templates/linkedin-with-alert.html`
- **Output:** `output/linkedin-banner.png`
- **Dimensions:** 1128x191px
- **Resolution:** 2x (2256x382px actual)
- **Features:**
  - Compact professional layout
  - Logo, brand name, and taglines on left
  - Alert card with process flow on right
  - Professional dark theme

### Facebook Cover (820x312px)
- **File:** `templates/facebook-with-alert.html`
- **Output:** `output/facebook-cover.png`
- **Dimensions:** 820x312px
- **Resolution:** 2x (1640x624px actual)
- **Safe Zone:** Center 640px (focus area for mobile)
- **Features:**
  - Centered layout for safe zone compatibility
  - Vertical divider separating brand and alert card
  - Optimized for mobile crop

### YouTube Banner (2560x1440px)
- **File:** `templates/youtube-with-alert.html`
- **Output:** `output/youtube-banner.png`
- **Dimensions:** 2560x1440px
- **Resolution:** 2x (5120x2880px actual)
- **Safe Zone:** 1546x423px (center)
- **Features:**
  - Large logo and brand name centered at top
  - Alert card with process flow in center
  - Social handles (@SigmatiqAI and sigmatiq.ai) on right
  - All important content within safe zone

### Discord Banner (960x540px)
- **File:** `templates/discord-with-alert.html`
- **Output:** `output/discord-banner.png`
- **Dimensions:** 960x540px
- **Resolution:** 2x (1920x1080px actual)
- **Features:**
  - Vertical layout with logo and brand at top
  - Alert card with full metrics and buttons
  - Process flow inside alert card
  - Community-friendly design

### Profile Picture (800x800px)
- **File:** `templates/profile-with-alert.html`
- **Output:** `output/profile-picture.png`
- **Dimensions:** 800x800px (square)
- **Resolution:** 2x (1600x1600px actual)
- **Features:**
  - Large centered logo at top
  - Brand name in middle
  - Alert card with full information at bottom
  - Optimized for circular cropping by platforms
  - Square format (platforms auto-crop to circle)

## Customization

### Editing Templates

All templates are standard HTML files with inline CSS. To customize:

1. Open the desired template in `templates/`
2. Edit HTML structure, text, colors, or layout
3. Save the file
4. Regenerate using `npm run generate:<platform>`

### Key Design Elements

**Logo:** Embedded inline SVG (teal corner blocks + golden radiation)

**Alert Card:** Semi-transparent card showing example options trade
- Symbol: AAPL 190C (weekly call option)
- Trade details: Premium, Contracts, Delta
- Action buttons: Approve/Decline
- Demonstrates product functionality

**Process Flow:** Three numbered circles with arrows
- 1. Paper (paper trading/simulation)
- 2. Practice (practice with guidance)
- 3. Live (live trading when ready)

**Background:** Dark gradient with subtle grid overlay and gradient orbs

**Typography:**
- Brand name: "SIGMA" (teal) + "TIQ" (golden)
- Tagline: "Your AI Trading Companion" (teal)
- Subtitle 1: "Built for Beginner Traders" (white/70% opacity)
- Subtitle 2: "Earn While You Learn" (golden)

### Changing Colors

Search and replace color values in HTML templates:

```css
#00C4A7  /* Teal - primary brand color */
#FFB800  /* Golden - accent color */
#0A1414  /* Dark - background start */
#152626  /* Dark - background end */
```

### Changing Text

Find and replace text in HTML templates:
- Brand name: `<span class="brand-teal">SIGMA</span><span class="brand-gold">TIQ</span>`
- Tagline: `Your AI Trading Companion`
- Subtitle 1: `Built for Beginner Traders`
- Subtitle 2: `Earn While You Learn`
- Alert symbol: `AAPL 190C` (example options trade)

## Technical Details

### Resolution and Quality

All templates are generated at **2x resolution** (deviceScaleFactor: 2) for:
- High-DPI displays (Retina, 4K)
- Sharp rendering on all devices
- Professional print quality if needed
- Better downscaling quality

### Browser Rendering

- **Engine:** Chromium (via Puppeteer)
- **Headless:** Yes
- **Wait Strategy:** `networkidle0` (wait for all resources)
- **Font Loading:** 1 second delay after page load for font rendering

### Output Format

- **Format:** PNG
- **Compression:** Standard PNG compression
- **Transparency:** No (solid background)
- **Color Space:** sRGB

## Platform Upload Guidelines

### Twitter/X
- **Dimensions:** 1500x500px minimum
- **Max File Size:** 5MB
- **Format:** PNG or JPG
- **Upload:** Profile → Edit Profile → Header Photo

### LinkedIn
- **Dimensions:** 1128x191px recommended
- **Max File Size:** 8MB
- **Format:** PNG or JPG
- **Upload:** Profile → Edit Background Photo

### Facebook
- **Dimensions:** 820x312px minimum
- **Max File Size:** 100KB
- **Format:** PNG or JPG
- **Safe Zone:** Center 640px (mobile view)
- **Upload:** Page → Edit Cover Photo

### YouTube
- **Dimensions:** 2560x1440px recommended
- **Safe Zone:** 1546x423px (center)
- **Max File Size:** 6MB
- **Format:** PNG or JPG
- **Upload:** Channel → Customize Channel → Branding → Banner Image

### Discord
- **Dimensions:** 960x540px recommended
- **Max File Size:** 10MB
- **Format:** PNG or JPG
- **Upload:** Server Settings → Overview → Server Banner
- **Note:** Requires boosted server (Level 2+)

### Profile Picture (All Platforms)
- **Dimensions:** 800x800px minimum
- **Format:** PNG (transparent) or JPG
- **Crop:** Most platforms crop to circle
- **Upload:** Platform-specific profile settings

## Troubleshooting

### Fonts Not Loading

If fonts appear incorrect:
1. Check internet connection (Google Fonts CDN)
2. Increase wait timeout in `generate-headers.js`
3. Download Inter font locally and reference in HTML

### Puppeteer Installation Issues

```bash
# Windows - use Git Bash or PowerShell
npm install puppeteer --legacy-peer-deps

# Linux - install dependencies
sudo apt-get install -y libgtk-3-0 libx11-xcb1 libnss3 libxss1 libasound2

# macOS - no additional dependencies needed
npm install
```

### Output Directory Missing

The script auto-creates `output/` directory. If issues persist:

```bash
mkdir output
```

### Memory Issues (YouTube Banner)

YouTube banner is large (2560x1440 @ 2x = 5120x2880). If memory errors occur:
1. Close other applications
2. Reduce `scale` in generate-headers.js (change from 2 to 1.5)
3. Generate YouTube separately: `npm run generate:youtube`

## Development

### Testing Templates Locally

Open HTML files directly in a browser:

```bash
# Windows
start templates/twitter.html

# macOS
open templates/twitter.html

# Linux
xdg-open templates/twitter.html
```

### Modifying Generator Script

The `generate-headers.js` script exports functions for programmatic use:

```javascript
const { generateHeader, generateAll } = require('./generate-headers.js');

// Generate single header
await generateHeader('twitter', browser);

// Generate all headers
await generateAll(browser);
```

### Adding New Templates

1. Create `templates/new-platform.html`
2. Add configuration to `TEMPLATES` object in `generate-headers.js`:

```javascript
newplatform: {
  name: 'New Platform',
  file: 'new-platform.html',
  output: 'new-platform-header.png',
  width: 1200,
  height: 400,
  scale: 2,
}
```

3. Add npm script to `package.json`:

```json
"generate:newplatform": "node generate-headers.js newplatform"
```

## Maintenance

### Updating Brand Colors

1. Edit color values in all HTML templates
2. Regenerate all headers: `npm run generate:all`
3. Review output files before uploading

### Updating Text/Messaging

1. Edit text in HTML templates
2. Regenerate specific headers or all
3. Test display on target platforms

### Logo Updates

If logo changes:
1. Update SVG in all template files (search for `<svg class="logo"`)
2. Alternatively, reference logo file URL
3. Regenerate all assets

## Best Practices

- **Always generate at 2x resolution** for best quality
- **Test on actual platforms** after generation (upload and preview)
- **Keep templates in sync** when making brand changes
- **Version control outputs** by dating or versioning folder
- **Backup templates** before major changes
- **Document customizations** in this README

## Support

For issues or questions:
- **GitHub:** Create issue in sigmatiq-orchestrator repo
- **Email:** support@sigmatiq.ai
- **Documentation:** See `sigmatiq-social-media-guide.md` in parent directory

## License

Copyright © 2025 SigmatiqAI. All rights reserved.

---

**Version:** 1.0.0
**Last Updated:** 2025-10-14
**Maintainer:** SigmatiqAI Team
