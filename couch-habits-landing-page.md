# Couchday — Landing Page Guide

**URL:** couchday.app

**Goal:** Get visitors to download the app

**Vibe:** Dark, calm, minimal — matches the app

---

## Page Structure

```
┌─────────────────────────────────────────────┐
│ Navigation                                  │
├─────────────────────────────────────────────┤
│ Hero                                        │
├─────────────────────────────────────────────┤
│ Problem                                     │
├─────────────────────────────────────────────┤
│ Solution                                    │
├─────────────────────────────────────────────┤
│ Features                                    │
├─────────────────────────────────────────────┤
│ Who It's For                                │
├─────────────────────────────────────────────┤
│ Screenshots                                 │
├─────────────────────────────────────────────┤
│ Download CTA                                │
├─────────────────────────────────────────────┤
│ Footer                                      │
└─────────────────────────────────────────────┘
```

---

## Section Copy

### Navigation

```
Logo: Couchday
Links: Features | Download
```

---

### Hero

**Headline:**
> Plan your day like a playlist.

**Subheadline:**
> No guilt. No pressure. Just a simple way to build and run your day — from the couch if you want.

**CTA Button:**
> Download on the App Store

[App Store badge]

[Hero image: App screenshot or device mockup]

---

### Problem

**Headline:**
> You've tried the other apps.

**Body:**
> The ones with streaks and badges and confetti explosions. You've set ambitious morning routines. You've told yourself "this time will be different."
>
> It wasn't. That's okay.

---

### Solution

**Headline:**
> Couch Habits is different.

**Body:**
> Miss a day? Nothing explodes. Your progress isn't lost. No streak shaming. No complicated stats. Just your habits, your pace.

[App screenshot showing gentle UI]

---

### Features

**Headline:**
> Simple by design.

**Features (icon + text):**

🛋️ **Daily & weekly habits**
Track what matters. Skip what doesn't.

✓ **Gentle streaks**
"5 days running" — not "YOU BROKE YOUR STREAK!"

📅 **Flexible scheduling**
Daily, 2x per week, whatever works.

🌙 **Calm dark interface**
Easy on the eyes. Easy on the mind.

📴 **Works offline**
No account. No sync. No fuss.

---

### Who It's For

**Headline:**
> Built for real life.

**List:**
- People who've quit every other habit app
- Overthinkers and procrastinators
- ADHD and neurodivergent brains
- Minimalists who want less, not more
- Anyone tired of feeling bad about missed days

---

### Screenshots

[3-4 app screenshots in a row or carousel]

**Caption (optional):**
> No graphs. No dashboards. Just your habits.

---

### Download CTA

**Headline:**
> Show up when you can. That's enough.

**CTA Button:**
> Download on the App Store

[App Store badge]

---

### Footer

```
Made with passion from the couch 🛋️

Links:
Privacy Policy | Terms | Contact

© 2026 Couch Habits
```

---

## Design Instructions

### Colors

| Element | Color |
|---------|-------|
| Background | #0a0a0f |
| Card background | #1a1a2e |
| Primary text | #ffffff |
| Secondary text | #ffffff (60% opacity) |
| Accent | #6c63ff |
| CTA button | #ffffff (text: #0a0a0f) |

### Typography

```
Font: Inter or SF Pro (system font)
Headline: 48-64px, bold, rounded
Subheadline: 20-24px, medium
Body: 16-18px, regular
```

### Spacing

```
Section padding: 80-120px vertical
Max content width: 1200px
Mobile: Stack everything, 24px padding
```

### Imagery

- Use device mockups with real screenshots
- Keep images dark to match theme
- Optional: Subtle gradient orbs in background (like your paywall)

---

## Build Options

| Tool | Effort | Cost |
|------|--------|------|
| Carrd | 30 min | $19/year |
| Framer | 1-2 hours | Free tier |
| Super (Notion) | 1 hour | $12/month |
| HTML/CSS | 2-3 hours | Free (host on Netlify) |
| Webflow | 1-2 hours | Free tier |

**Recommendation:** Carrd for speed, Framer for polish.

---

## SEO Basics

```
Title: Couch Habits — The Gentle Habit Tracker
Description: The habit tracker that expects nothing from you. No guilt. No pressure. Build habits from the couch.
```

---

## Checklist

- [ ] Domain connected (couchhabits.app)
- [ ] SSL enabled (https)
- [ ] App Store link added
- [ ] Privacy policy page
- [ ] Mobile responsive
- [ ] Open Graph image (for social sharing)
- [ ] Favicon (🛋️ or app icon)

---

## Open Graph (Social Sharing)

Add these meta tags for proper social sharing:

```html
<meta property="og:title" content="Couch Habits — The Gentle Habit Tracker">
<meta property="og:description" content="The habit tracker that expects nothing from you. No guilt. No pressure.">
<meta property="og:image" content="https://couchhabits.app/og-image.png">
<meta property="og:url" content="https://couchhabits.app">
<meta name="twitter:card" content="summary_large_image">
```

**OG Image specs:**
- Size: 1200 x 630px
- Include: App name, tagline, device mockup
- Dark background to match brand
