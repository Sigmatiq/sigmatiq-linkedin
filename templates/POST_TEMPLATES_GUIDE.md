# Social Media Post Templates - Usage Guide

This guide explains how to customize and use the three post templates for SigmatiqAI social media content.

---

## 🎯 Ready-to-Use Sample Posts (Examples)

We've created **3 sample post images** to demonstrate what you can create with these templates:

| Sample Image | Template Type | Theme |
|--------------|---------------|-------|
| `output/posts/monday-motivation.png` | Educational | Monday Motivation |
| `output/posts/risk-management.png` | Educational | Risk Management |
| `output/posts/beta-waitlist.png` | Announcement | Beta Testing CTA |

**Important:** These are just examples. You'll create NEW images for your actual posts by customizing the templates below.

**Relationship with SOCIAL_MEDIA_POSTS.md:**
- **SOCIAL_MEDIA_POSTS.md** = Text captions for text-only posts OR captions that accompany images
- **These Templates** = Visual image posts that pair WITH text captions or stand alone
- Many posts in SOCIAL_MEDIA_POSTS.md are text-only and don't need images
- Use these templates when you want to create eye-catching visual posts

---

## 📁 Template Files

All templates are located in the `templates/` folder:

| Template File | Output Image | Use Case |
|---------------|--------------|----------|
| `post-educational.html` | `output/post-educational.png` | Trading tips, motivation, educational content |
| `post-product-feature.html` | `output/post-product-feature.png` | Product features, how-to guides, UI showcases |
| `post-announcement.html` | `output/post-announcement.png` | Announcements, beta testing, CTAs, updates |

**Image Specifications:**
- **Dimensions:** 1080x1080px (square format)
- **Resolution:** 2x (high quality for social media)
- **Format:** PNG
- **Platforms:** Works on Instagram, Twitter/X, Facebook, LinkedIn

---

## 🎨 Template 1: Educational Posts

**Best for:** Monday Motivation, Trading Education, Risk Management tips, Quotes, General advice

### What to Customize:

#### 1. Category Tag
```html
<div class="category-tag">Trading Education</div>
```
**Options:**
- `Trading Education`
- `Monday Motivation`
- `Risk Management`
- `Trading Psychology`
- `Trading Tips`

#### 2. Main Quote/Headline
```html
<div class="main-quote">
    Successful trading isn't about being <span class="highlight">right 100%</span> of the time
</div>
```
**Tips:**
- Keep it punchy (10-15 words max)
- Use `<span class="highlight">` to emphasize key phrases in gold color
- Make it quotable and shareable

#### 3. Supporting Text
```html
<div class="sub-text">
    It's about cutting losses quickly, letting winners run, staying disciplined, and learning from every trade.
</div>
```
**Tips:**
- 1-2 sentences max
- Explains or supports the main headline
- Keep it under 150 characters

### Example Variations:

**Example 1: Risk Management**
```html
<div class="category-tag">Risk Management</div>
<div class="main-quote">
    Never risk more than <span class="highlight">1-2%</span> per trade
</div>
<div class="sub-text">
    Small losses are recoverable. Large losses end accounts. Our AI enforces this automatically.
</div>
```

**Example 2: Monday Motivation**
```html
<div class="category-tag">Monday Motivation</div>
<div class="main-quote">
    The best traders aren't the <span class="highlight">smartest</span>—they're the most <span class="highlight">disciplined</span>
</div>
<div class="sub-text">
    Stick to your system. Trust your process. Let the AI help you stay consistent.
</div>
```

---

## 🎯 Template 2: Product Feature Posts

**Best for:** How features work, Alert card showcases, UI demonstrations, Product explanations

### What to Customize:

#### 1. Feature Title
```html
<div class="feature-title">How Our Paper Trading Works</div>
```
**Options:**
- `How Our Paper Trading Works`
- `AI Model Selection Explained`
- `5-Layer Safety System`
- `Your First Alert Walkthrough`
- `Understanding Risk Management`

#### 2. Feature Subtitle
```html
<div class="feature-subtitle">Choose your AI model, get alerts, approve trades—zero risk</div>
```
**Tips:**
- Short summary of the feature (under 80 characters)
- Highlights the key benefit

#### 3. Alert Card Details

**Symbol & Price:**
```html
<div class="symbol">AAPL 190C</div>
<div class="price">• Fri (weekly)</div>
```

**Time Badge:**
```html
<div class="badge">02:00</div>
```
Change to show time remaining or other badge text

**Description:**
```html
<div class="alert-description">
    Day-trade call, liquid weekly, tight spread, ~0.4 delta
</div>
```

**Metrics:**
```html
<div class="metric">
    <div class="metric-label">Premium:</div>
    <div class="metric-value positive">$0.43 (spread ~$0.02)</div>
</div>
```
**Metric classes:**
- `.positive` = Green text (#00D4AA)
- `.negative` = Red text (#FF6B6B)
- No class = White text

**Reasoning Box:**
```html
<div class="alert-reason">
    <strong>Why this setup:</strong> Bullish momentum on AAPL, approaching resistance with strong volume. Target quick 20-30% gain on premium.
</div>
```

### Example Variations:

**Example 1: Safety Features**
```html
<div class="feature-title">5-Layer Safety System</div>
<div class="feature-subtitle">Protecting beginners from devastating losses</div>

<!-- Modify alert card to show safety features instead of trade details -->
<!-- For example, list the 5 layers in the metrics section -->
```

**Example 2: AI Model Selection**
```html
<div class="feature-title">Choose Your AI Model</div>
<div class="feature-subtitle">Conservative, Balanced, or Aggressive—match your risk tolerance</div>

<!-- Show a conservative trade example in the alert card -->
```

---

## 📢 Template 3: Announcement Posts

**Best for:** Beta testing, Launch announcements, Waitlist CTAs, Development updates, Milestones

### What to Customize:

#### 1. Announcement Label
```html
<div class="announcement-label">Beta Testing</div>
```
**Options:**
- `Beta Testing`
- `Now Launching`
- `Coming Soon`
- `New Feature`
- `Big Update`
- `Milestone`

#### 2. Main Headline
```html
<div class="main-headline">
    Join the <span class="gradient-text">First 100</span> Beta Testers
</div>
```
**Tips:**
- Use `<span class="gradient-text">` to apply teal-to-gold gradient to key words
- Keep it bold and attention-grabbing
- 5-10 words max

#### 3. Description
```html
<div class="description">
    Test all features, shape the product, and get free premium access to your AI trading companion.
</div>
```
**Tips:**
- Explain the value/benefit
- 1-2 sentences
- Under 150 characters

#### 4. CTA Button
```html
<div class="cta-button">Join Waitlist</div>
```
**Options:**
- `Join Waitlist`
- `Get Early Access`
- `Sign Up Now`
- `Learn More`
- `Download Now`

#### 5. CTA Subtext
```html
<div class="cta-subtext">Limited spots available</div>
```
**Options:**
- `Limited spots available`
- `First 100 users only`
- `Beta testing starts soon`
- `Free for early adopters`

### Example Variations:

**Example 1: Launch Announcement**
```html
<div class="announcement-label">Now Launching</div>
<div class="main-headline">
    SigmatiqAI is <span class="gradient-text">Live</span>
</div>
<div class="description">
    Your AI Trading Companion is ready. Start with paper trading today—zero risk, unlimited learning.
</div>
<div class="cta-button">Start Now</div>
<div class="cta-subtext">Paper trading always available</div>
```

**Example 2: New Feature**
```html
<div class="announcement-label">New Feature</div>
<div class="main-headline">
    Practice Mode <span class="gradient-text">Now Available</span>
</div>
<div class="description">
    Proven profitable in paper trading? Upgrade to practice mode and earn while you learn with small real capital.
</div>
<div class="cta-button">Learn More</div>
<div class="cta-subtext">For verified paper traders</div>
```

---

## 🛠️ How to Generate Images

### Step 1: Edit the HTML Template

1. Open the template file in a text editor (VS Code recommended)
2. Find the sections marked in this guide
3. Replace the text with your content
4. Save the file

### Step 2: Generate the Image

**Option A: Generate Single Template**

Create a new script or modify `generate-posts.js` to generate just one:

```bash
node generate-posts.js
```

**Option B: Generate All Templates**

Run the existing script to regenerate all three:

```bash
cd C:\Sigmatiq\Dev-1\social-media-branding
node generate-posts.js
```

**Option C: Open in Browser (Preview Only)**

1. Open the HTML file directly in a browser
2. Take a screenshot manually
3. Crop to 1080x1080px

### Step 3: Use the Generated Image

Your image will be in the `output/` folder:
- `output/post-educational.png`
- `post/product-feature.png`
- `output/post-announcement.png`

---

## 🎨 Design Guidelines

### Color Usage

**Primary Colors:**
- **Teal:** `#00C4A7` - Logo, highlights, positive metrics
- **Gold:** `#FFB800` - Logo, highlights, important text
- **Dark Teal:** `#0a2828` to `#1a3838` - Background gradients

**Text Colors:**
- **White:** `#ffffff` - Main headlines
- **Light Gray:** `rgba(255, 255, 255, 0.7)` - Body text
- **Subtle Gray:** `rgba(255, 255, 255, 0.5)` - Labels, subtext

**Accent Colors:**
- **Green (Positive):** `#00D4AA` - Gains, positive metrics
- **Red (Negative):** `#FF6B6B` - Losses, negative metrics

### Typography

**Font Family:** Inter (fallback to system fonts)

**Font Sizes:**
- **Educational Template:**
  - Category tag: 16px
  - Main quote: 56px
  - Sub-text: 24px

- **Product Feature Template:**
  - Feature title: 48px
  - Feature subtitle: 22px
  - Alert card text: 16-32px (varies)

- **Announcement Template:**
  - Label: 18px
  - Headline: 72px
  - Description: 26px
  - CTA button: 22px

### Logo

All templates use the correct SVG logo:
- 3x3 grid pattern
- Top-left 2x2: Teal squares
- Center radiating: Gold squares
- Consistent across all templates

### Footer

All templates include `sigmatiq.ai` in the bottom center:
- Font size: 18px
- Color: `rgba(255, 255, 255, 0.35)`
- Position: 50px from bottom

---

## 📋 Content Strategy: When to Use Templates vs Text-Only

### Text-Only Posts (from SOCIAL_MEDIA_POSTS.md)
Use text captions without images for:
- **Twitter/X threads** - Multi-tweet explanations work better as pure text
- **LinkedIn long-form posts** - Professional insights and thought leadership
- **Facebook detailed posts** - Community engagement and discussions
- **Quick updates** - Development updates, FAQs, simple announcements

**Examples from SOCIAL_MEDIA_POSTS.md that are text-only:**
- Post 1: Introduction (LinkedIn long-form explanation)
- Post 2: How Paper Trading Works (detailed Twitter thread)
- Post 3: Three-Step Journey (educational thread)
- Post 6: 5-Layer Safety System (Twitter thread)
- Post 7: FAQ posts

### Visual Posts (using these templates)
Create custom images when you want:
- **High visual impact** - Grab attention in feeds
- **Stand-out quotes** - Make quotes shareable
- **Brand consistency** - Show professional design
- **Instagram/visual platforms** - Required for Instagram posts
- **Highlight key messages** - Single powerful statement

**Best Template Choices:**
| Content Type | Template | When to Create | Pair With |
|--------------|----------|----------------|-----------|
| Monday Motivation | Educational | Weekly (Mondays) | Short caption from SOCIAL_MEDIA_POSTS.md |
| Trading tips | Educational | 2-3x per week | Educational section captions |
| Risk management | Educational | Weekly | Text explanation in caption |
| Feature showcase | Product Feature | 1x per week | How-to caption |
| Alert examples | Product Feature | 2x per week | Brief explanation |
| Beta announcements | Announcement | As needed | Waitlist CTA text |
| Launch news | Announcement | Major milestones | Launch post caption |
| New features | Announcement | When shipping | Feature details in caption |

### Recommended Mix
- **70% Text-Only** - Use captions from SOCIAL_MEDIA_POSTS.md as-is
- **30% Visual** - Create custom images using these templates for high-impact posts

This keeps your feed fresh, diverse, and not overly "designed" (which can feel less authentic).

---

## ✅ Pre-Flight Checklist

Before generating and posting:

- [ ] Content is accurate and fact-checked
- [ ] Text fits within character limits
- [ ] Highlighted text uses `<span class="highlight">` or `<span class="gradient-text">`
- [ ] Alert card metrics are realistic (if using product template)
- [ ] CTA is clear and actionable (if using announcement template)
- [ ] Logo displays correctly
- [ ] Website footer shows `sigmatiq.ai`
- [ ] Generated image is 1080x1080px
- [ ] No typos or grammatical errors
- [ ] Compliant with trading disclosure requirements (if showing performance)

---

## 🚨 Compliance Notes

**When showing trade examples or performance:**

Always include this disclaimer in your post caption:
```
⚠️ Disclosure: Trading involves risk. Paper trading results are simulated and don't represent real trading. Past performance doesn't guarantee future results. Not financial advice.
```

**Do NOT:**
- Show real account balances
- Guarantee profits or returns
- Make unrealistic claims
- Use misleading performance data

---

## 💡 Pro Tips

1. **Batch Content Creation:** Edit all three templates at once for the week, then generate all images together

2. **Seasonal Variations:** Update colors slightly for holidays (keep brand consistency but add seasonal touches)

3. **A/B Testing:** Create two versions of the same content with different headlines to see what performs better

4. **Reuse Templates:** Save your best-performing edits as separate HTML files (e.g., `post-educational-monday-motivation.html`)

5. **Keep it Fresh:** Rotate between all three templates to keep your feed visually interesting

6. **Pair with SOCIAL_MEDIA_POSTS.md:** Use the ready-to-post content from that document, then create matching visuals with these templates

---

## 📞 Need Help?

If you encounter issues:

1. **Template not generating?**
   - Check that Node.js and Puppeteer are installed
   - Run `npm install` in the social-media-branding folder

2. **Image looks wrong?**
   - Open HTML file in Chrome/Edge to preview
   - Check for unclosed HTML tags
   - Validate that all CSS classes are correct

3. **Want to add new templates?**
   - Duplicate an existing template
   - Modify the layout and content
   - Add to `generate-posts.js` array

---

*Last Updated: 2025*
*Version: 1.0*
