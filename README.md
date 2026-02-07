# 💕 Will You Be My Valentine? Website

An ultra-interactive, multi-screen Valentine's Day experience with games, animations, and surprises at every turn! This isn't just a question - it's a journey through your feelings! 🎉

---

## 👨‍💻 Author

**Sohom Banerjee**

| Platform | Link |
|----------|------|
| 🐙 GitHub | [github.com/Srap47](https://github.com/Srap47) |
| 📧 Email | [sohommister@gmail.com](mailto:sohommister@gmail.com) |
| 💼 LinkedIn | [linkedin.com/in/sohom-banerjee-863775225](https://www.linkedin.com/in/sohom-banerjee-863775225/) |

---

## 🏗️ Project Architecture

### Overview

This is a **single-page application (SPA)** built with vanilla HTML, CSS, and JavaScript. No frameworks or build tools required - just pure web technologies for maximum compatibility and easy deployment.

```
┌─────────────────────────────────────────────────────────────────┐
│                        BROWSER CLIENT                           │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌─────────────┐    ┌─────────────┐    ┌─────────────┐        │
│  │   Screen 1  │───▶│   Screen 2  │───▶│   Screen 3  │        │
│  │  (Welcome)  │    │  (Reasons)  │    │ (Question)  │        │
│  └─────────────┘    └─────────────┘    └──────┬──────┘        │
│                                                │                │
│                                                ▼                │
│                                         ┌─────────────┐        │
│                                         │   Screen 4  │        │
│                                         │(Celebration)│        │
│                                         └─────────────┘        │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                      CORE MODULES                               │
├──────────────┬──────────────┬──────────────┬───────────────────┤
│  Animation   │    Audio     │    Game      │   Navigation      │
│   Engine     │   Manager    │   Logic      │    Controller     │
├──────────────┼──────────────┼──────────────┼───────────────────┤
│ • Confetti   │ • Play/Pause │ • Heart Grid │ • Screen Switch   │
│ • Fireworks  │ • Loop       │ • Love Calc  │ • Nav Dots        │
│ • Hearts     │ • Volume     │ • Carousel   │ • Button States   │
│ • Cursor     │              │ • Letters    │                   │
└──────────────┴──────────────┴──────────────┴───────────────────┘
```

### Technology Stack

| Layer | Technology | Purpose |
|-------|------------|---------|
| **Structure** | HTML5 | Semantic markup, multi-screen layout |
| **Styling** | CSS3 | Animations, gradients, responsive design |
| **Logic** | Vanilla JavaScript | Interactivity, game mechanics, effects |
| **Fonts** | Google Fonts | Pacifico, Quicksand, Dancing Script |
| **Hosting** | GitHub Pages | Free static site hosting |

### Design Patterns Used

- **State Machine**: Screen navigation (4 states/screens)
- **Observer Pattern**: Event listeners for user interactions
- **Module Pattern**: Encapsulated functions for each feature

---

## 📁 File Architecture

```
love-website/
│
├── 📄 index.html          # Main application file (single-file architecture)
│   │
│   ├── <head>
│   │   ├── Meta tags & viewport settings
│   │   ├── Google Fonts imports
│   │   └── <style> - All CSS (800+ lines)
│   │       ├── CSS Variables (color palette)
│   │       ├── Base styles & resets
│   │       ├── Component styles
│   │       │   ├── Loading screen
│   │       │   ├── Music control button
│   │       │   ├── Navigation dots
│   │       │   ├── Floating hearts
│   │       │   ├── Card container
│   │       │   ├── Love letter section
│   │       │   ├── Love calculator
│   │       │   ├── Reasons section
│   │       │   ├── Memory carousel
│   │       │   ├── Hearts grid game
│   │       │   ├── Button styles
│   │       │   └── Success screen
│   │       ├── Animation keyframes
│   │       │   ├── @keyframes float
│   │       │   ├── @keyframes heartbeat
│   │       │   ├── @keyframes bounce
│   │       │   ├── @keyframes pulse
│   │       │   ├── @keyframes confetti-fall
│   │       │   └── @keyframes fireworkExplode
│   │       └── Responsive media queries
│   │
│   ├── <body>
│   │   ├── Loading screen overlay
│   │   ├── Music control button (fixed)
│   │   ├── Navigation dots (fixed)
│   │   ├── Floating hearts container
│   │   └── Main container
│   │       ├── Screen 1: Welcome
│   │       │   ├── Title & subtitle
│   │       │   ├── Love letter generator
│   │       │   └── "See Why You're Special" button
│   │       │
│   │       ├── Screen 2: Reasons
│   │       │   ├── Animated reasons list (5 items)
│   │       │   ├── Love calculator with meter
│   │       │   ├── Memory carousel (5 slides)
│   │       │   └── "Ready to Answer?" button
│   │       │
│   │       ├── Screen 3: The Question
│   │       │   ├── Hearts grid game (6 hearts)
│   │       │   ├── Hidden question message
│   │       │   └── Yes/No buttons (hidden initially)
│   │       │
│   │       └── Screen 4: Celebration
│   │           ├── Success message
│   │           ├── Rotating couple emoji
│   │           ├── 100% love meter
│   │           └── "Start Over" button
│   │
│   └── <script> - All JavaScript (400+ lines)
│       ├── Loading screen handler
│       ├── Cursor trail effect
│       ├── Clickable hearts with burst effect
│       ├── Music control (Audio API)
│       ├── Love letter generator (20 messages)
│       ├── Screen navigation system
│       ├── Love calculator animation
│       ├── Memory carousel auto-scroll
│       ├── Heart revealing game logic
│       ├── "No" button behavior (shrink & move)
│       ├── "Yes" handler with celebrations
│       ├── Confetti effect generator
│       └── Fireworks effect generator
│
├── 🎵 song.mp3             # Background music file (user-provided)
│   └── Recommended: <25MB, romantic song
│
└── 📖 README.md            # Project documentation (this file)
```

### Code Statistics

| Metric | Count |
|--------|-------|
| Total Lines | ~1,450 |
| CSS Lines | ~800 |
| JavaScript Lines | ~400 |
| HTML Lines | ~250 |
| Animations | 12 |
| Screens | 4 |
| Interactive Elements | 15+ |

---

## 🌟 Features

### 🎨 Visual Effects
- **Beautiful gradient background** with purple and pink tones
- **Floating animated hearts** that you can click for burst effects
- **Cursor trail effects** that follow your mouse (desktop only)
- **Loading screen animation** for a polished entrance
- **Confetti & fireworks** celebration effects
- **Smooth animations** and transitions throughout
- **Custom fonts** from Google Fonts (Pacifico, Quicksand & Dancing Script)

### 🎮 Interactive Elements
- **Multi-screen experience** - Navigate through 4 different screens
- **Love letter generator** with 20 unique romantic messages
- **Love calculator** with animated progress bar (always shows 99% compatibility 😉)
- **Auto-scrolling memory carousel** with 5 romantic moments
- **Heart-revealing game** - Click all 6 hearts to unlock the final question
- **Side navigation dots** to track your progress (desktop)
- **Music toggle button** with background romantic music support
- **Interactive "No" button** that shrinks, moves, and tries to convince them with 12 different messages
- **Clickable floating hearts** that explode into mini hearts

### 📱 Multi-Screen Journey
1. **Screen 1: Welcome** - Love letter generator and initial greeting
2. **Screen 2: Why You're Special** - Animated reasons list, love calculator, and memory carousel
3. **Screen 3: The Big Question** - Interactive heart game before the proposal
4. **Screen 4: Celebration** - Massive celebration with confetti, fireworks, and 100% love score

---

## 🚀 Deployment Guide

### Quick Deploy to GitHub Pages

**Step 1: Create Repository**
```bash
# Create a new repo on github.com named "valentine" or similar
# Make it PUBLIC for GitHub Pages to work
```

**Step 2: Upload Files**
1. Go to your repository on GitHub
2. Click "Add file" → "Upload files"
3. Drag and drop:
   - `index.html`
   - `song.mp3` (your romantic song, renamed to song.mp3)
4. Click "Commit changes"

**Step 3: Enable GitHub Pages**
1. Go to repository **Settings**
2. Click **Pages** in the left sidebar
3. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
4. Click **Save**

**Step 4: Access Your Site**
- Wait 1-2 minutes for deployment
- Your site will be live at: `https://YOUR-USERNAME.github.io/REPO-NAME/`

### Using Git CLI

```bash
# Clone your new repository
git clone https://github.com/YOUR-USERNAME/valentine.git
cd valentine

# Copy your files (index.html, song.mp3) to this directory

# Commit and push
git add .
git commit -m "Add Valentine's Day website"
git push origin main

# Then enable GitHub Pages in repository settings
```

---

## 🎵 Adding Background Music

1. **Get your song**: Download an MP3 of your special song
2. **Rename it**: Change the filename to `song.mp3`
3. **Place it**: Put it in the same folder as `index.html`
4. **Test it**: Open `index.html` in a browser and click the 🎵 button

> **Note**: Keep the MP3 under 25MB for fast loading. GitHub allows up to 100MB per file.

---

## 🎨 Customization

### Change Messages

**Love letter messages** (in JavaScript, line ~1149):
```javascript
const loveLetters = [
    "Your custom message here...",
    // Add more messages
];
```

**Reasons list** (in HTML, line ~891):
```html
<div class="reason-item">
    <span class="reason-emoji">😊</span>
    <span>Your custom reason here!</span>
</div>
```

### Change Colors

Edit CSS variables (line ~11):
```css
:root {
    --rose: #ff6b9d;
    --blush: #ffc2d4;
    --cream: #fff5f7;
    --burgundy: #c23866;
    --gold: #ffd700;
    --purple: #667eea;
}
```

### Change "No" Button Responses

Edit the array (line ~1330):
```javascript
const noBtnTexts = [
    "No",
    "Are you sure bujiluu? 🥺",
    "clingyyy![IMG_20251123_204739_112](https://github.com/user-attachments/assets/f55b2741-5120-48ed-ba02-06e2826daece)
![IMG_20251123_204739_112](https://github.com/user-attachments/assets/a4995a06-fc55-4606-b464-766e8f000df7)
 please? 🙏",
    // Add your own messages!
];
```

---

## 📱 Responsive Design

The website is fully responsive and tested on:
- 📱 Mobile phones (320px+)
- 📱 Tablets (768px+)
- 💻 Laptops (1024px+)
- 🖥️ Large desktops (1440px+)

---

## 🎉 What Happens When They Click "Yes"

1. Navigate to celebration screen
2. Beautiful success message with color-changing title
3. **Massive confetti explosion** (100 pieces!)
4. **5 firework bursts** with 30 particles each
5. Animated rotating couple emoji
6. **100% love compatibility meter**
7. Option to restart the experience

---

## 💡 Tips for the Best Experience

- **Desktop viewing recommended** for cursor trails and full navigation
- **Test all screens** before sharing to verify music works
- The journey takes about 2-3 minutes if explored fully
- **Send at a special time**: midnight, morning surprise, Valentine's Day!
- Use a URL shortener like [bit.ly](https://bit.ly) for a cleaner link

---

## 📝 License

This project is open source and available for personal use. Feel free to customize it for your Valentine! ❤️

---

<p align="center">
Made with 💕 by <a href="https://github.com/Srap47">Sohom Banerjee</a>
</p>
git clone https://github.com/Srap47/be-my-valentine.git
cd be-my-valentine
# Replace photo.jpg with your new image (make sure it's named photo.jpg)
git add photo.jpg
git commit -m "Replace photo with new image"
git push origin main![IMG_20251123_204739_112](https://github.com/user-attachments/assets/53e00a59-c198-4071-be9e-91a97c3c2e4c)
<img width="641" height="641" alt="image" src="https://github.com/user-attachments/assets/bf820919-ae43-4d52-b602-0c66507bd0bb" />

